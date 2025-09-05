<div align="center">
  <h1>Aplicativo de Gestão Administrativa - Guarnição de Caçapava</h1>
  <h3>Projeto de API - Fatec Prof° Jessen Vidal - 2º Semestre de 2025</h3>
</div>

<p align="center">
  Projeto acadêmico desenvolvido por alunos do 5º semestre de DSM. O objetivo é digitalizar e automatizar
  a gestão de almoxarifado, substituindo controles manuais e descentralizados que dificultam o rastreamento
  de itens e impactam a eficiência operacional.
</p>

<div align="center">

![Badge](https://img.shields.io/badge/status-planejamento-lightgrey)
![Badge](https://img.shields.io/badge/metodologia-Scrum-blue)

</div>

---

## 🗂️ Índice
- [Metodologia Utilizada](#-metodologia-utilizada)
- [Tecnologias Utilizadas](#️-tecnologias-utilizadas)
- [Requisitos do Projeto](#-requisitos-do-projeto)
- [Product Backlog](#-product-backlog)
- [Backlog da Sprint](#-backlog-da-sprint)
- [DoR (Definition of Ready)](docs/dor.md)
- [DoD (Definition of Done)](docs/dod.md)
- [Manual de Instalação](docs/manual-de-instalacao.md)
- [Manual do Usuário](docs/manual-do-usuario.md)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Estratégia de Branching](docs/estrategia-de-branch.md)
- [Padrão de Commit](docs/padrao-de-commits.md)
- [Integrantes do Grupo](#-integrantes-do-grupo)

---

## 📋 Metodologia Utilizada

O framework de Metodologia Ágil utilizado no produto foi o **Scrum**, um método adaptativo, iterativo e eficaz para a gestão de projetos. O trabalho é organizado em Sprints, com cerimônias como Planejamento (Planning), Execuções Diárias (Dailies) e Revisões (Review) para garantir entregas de valor contínuas e alinhadas às necessidades do cliente.

---

## 🖥️ Tecnologias Utilizadas

Estas foram as tecnologias escolhidas para a produção do projeto:

<div align="center">
  <a href="https://flutter.dev/"><img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white"/></a>
  <a href="https://nodejs.org/"><img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white"/></a>
  <a href="https://www.postgresql.org/"><img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/></a>
  <a href="https://git-scm.com/"><img src="https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white"/></a>
  <a href="https://www.java.com/"><img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white"/></a>
  <a href="https://discord.com/"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white"/></a>
</div>

---

## 📖 Requisitos do Projeto

### Requisitos Funcionais

| Id   | Requisito Funcional                                                                                                                              |
| :--- | :----------------------------------------------------------------------------------------------------------------------------------------------- |
| RF01 | **Gestão de Itens:** Permitir o cadastro, edição e consulta de itens, incluindo nome, descrição, unidade de medida e estoque mínimo.               |
| RF02 | **Controle de Entradas e Saídas:** Registrar a entrada de novos materiais e a saída por requisição, atualizando o estoque em tempo real.           |
| RF03 | **Rastreabilidade com QR Code:** Gerar e ler QR Codes para identificar e consultar informações de itens rapidamente.                               |
| RF04 | **Alertas de Estoque Mínimo:** Notificar gestores quando um item atingir o nível de estoque mínimo pré-definido.                                    |
| RF05 | **Autenticação e Perfis de Acesso:** Implementar login e perfis de usuário (administrador, operador) com permissões específicas.                   |
| RF06 | **Relatórios Gerenciais:** Gerar relatórios sobre o status do inventário, movimentações por período e itens abaixo do mínimo.                      |
| RF07 | **Fonte de Dados Externos (Nota Fiscal):** Importar/integar com fonte de notas fiscais eletrônicas para reconciliar entradas e fornecedores.        |
| RF08 | **Envio de Alertas por E-mail (EBmail):** Disparar e-mails funcionais para gestores/fornecedores (alertas de estoque, confirmação de pedido, etc.).  |

### Requisitos Não Funcionais

| Id    | Requisito Não Funcional                                                                                                                     |
| :---- | :------------------------------------------------------------------------------------------------------------------------------------------ |
| RNF01 | **Usabilidade:** A interface deve ser intuitiva e de fácil utilização, com um mínimo de treinamento necessário.                             |
| RNF02 | **Performance:** Operações críticas (leitura de QR Code, atualização de estoque) devem ser concluídas rapidamente.               |
| RNF03 | **Segurança:** A comunicação entre app e API deve ser criptografada (HTTPS). Senhas devem ser armazenadas com hash.                         |
| RNF04 | **Manual de Instalação:** Documentação passo-a-passo para configurar ambiente de desenvolvimento e produção (docs/manual-de-instalacao.md). |
| RNF05 | **Manual do Usuário:** Guia de funcionalidades e fluxos do usuário (docs/manual-do-usuario.md).                                             |
| RNF06 | **Compatibilidade:** O aplicativo móvel deve ser compatível com as duas últimas versões dos sistemas operacionais Android e iOS.            |

---

## 📒 Product Backlog
> Em desenvolvimento.

--- 

## 📆 Backlog da Sprint
> Em desenvolvimento.

---

## ✅ Checklist de DoR
Checklist resumido — para a versão completa e imprimível, consulte:  
[📄 Definition of Ready (DoR) — docs/dor.md](docs/dor.md)

---

## ✅ Definition of Done (DoD)
Critérios de aceitação e qualidade para encerrar uma issue/PR:  
[📄 Definition of Done (DoD) — docs/dod.md](docs/dod.md)

---

## 🚀 Como Começar

Para configurar o ambiente de desenvolvimento local, siga os passos abaixo.

---

## 📖 Manual do Usuário
1. O usuário deve se autenticar com login e senha.  
2. Gestores podem cadastrar itens e gerar relatórios.  
3. Operadores podem registrar entradas e saídas.  
4. O app permite consultar itens via **QR Code**.  
5. Notificações são enviadas quando estoque atinge o mínimo.  

### Pré-requisitos

Instale/configure localmente antes de iniciar:

| Componente | Versão / Observação | Verificação rápida |
|------------|---------------------|--------------------|
| Git | Última versão estável | git --version |
| Node.js + npm | LTS (ex: 20.x) | node -v / npm -v |
| PostgreSQL | 15+ (ou usar Docker) | psql --version |
| Flutter SDK | Versão estável atual | flutter --version |
| Dart (incluso no Flutter) | Bundled | dart --version |
| Java JDK | 17 (necessário para build Android) | java -version |
| Android Studio (SDK / AVD) | Atual | flutter doctor |
| VS Code (ou IDE preferida) | Extensões: Flutter, Dart | code -v |


## 📂 Estrutura do Projeto

> Em desenvolvimento.

---

## 🙎 Integrantes do Grupo

<div align="center">

|          |   Nome   |  Função  |  GitHub  | LinKedin |
| :------: | :------: | :------: | :------: | :------: |
| <img src="https://avatars.githubusercontent.com/u/142221532?v=4" alt="foto de perfil" height="64px" width="64px"> | Renato Cruz | Scrum Master | <a href="https://github.com/Renato-Cruz-Jr"><img src="https://img.shields.io/badge/GitHub-13196a?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/renato-fernandes-da-cruz-junior-798582204/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
| <img src="https://avatars.githubusercontent.com/u/142221848?v=4" alt="foto de perfil" height="64px" width="64px"> | Jonas Miguel | Product Owner | <a href="https://github.com/Jonasoliver"><img src="https://img.shields.io/badge/GitHub-13196a?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/jonas-miguel-ol"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
| <img src="https://avatars.githubusercontent.com/u/104574671?v=4" alt="foto de perfil" height="64px" width="64px"> | Davi Maciel | Developer | <a href="https://github.com/DfMaciel"><img src="https://img.shields.io/badge/GitHub-13196a?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/dfmaciel"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
| <img src="https://avatars.githubusercontent.com/u/61799878?v=4" alt="foto de perfil" height="64px" width="64px"> | Elisa Rachel | Developer | <a href="https://github.com/elisarachel"><img src="https://img.shields.io/badge/GitHub-13196a?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/elisa-beninca-704566292/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
| <img src="https://avatars.githubusercontent.com/u/142221695?v=4" alt="foto de perfil" height="64px" width="64px"> | Joyce Silva | Developer | <a href="https://github.com/joycesilvaaa"><img src="https://img.shields.io/badge/GitHub-13196a?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/joyce-silva-79a4b9287/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
| <img src="https://avatars.githubusercontent.com/u/142221388?v=4" alt="foto de perfil" height="64px" width="64px"> | Júlia Rosado | Developer | <a href="https://github.com/juliamariahr"><img src="https://img.shields.io/badge/GitHub-13196a?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/júlia-rosado/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
| <img src="https://avatars.githubusercontent.com/u/142221456?v=4" alt="foto de perfil" height="64px" width="64px"> | Pedro Oliveira | Developer | <a href="https://github.com/OliveiraPedro09"><img src="https://img.shields.io/badge/GitHub-13196a?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/pedrooliv9"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
| <img src="https://avatars.githubusercontent.com/u/79583088?v=4"  alt="foto de perfil" height="64px" width="64px"> | Yuri Braga | Developer | <a href="https://github.com/yuribragga"><img src="https://img.shields.io/badge/GitHub-13196a?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/yuri-braga/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |

</div>


---

<div align="center">
  <b>Desenvolvido pela equipe <a href="https://github.com/Code-Nine-FTC">Code Nine</a></b>
</div>