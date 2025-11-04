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

![Badge](https://img.shields.io/badge/status-Em%20andamento-yellow)
![Badge](https://img.shields.io/badge/metodologia-Scrum-blue)

</div>

---

## 🗂️ Índice
- [Metodologia Utilizada](#-metodologia-utilizada)
- [Tecnologias Utilizadas](#️-tecnologias-utilizadas)
- [Requisitos do Projeto](#-requisitos-do-projeto)
- [Product Backlog](#-product-backlog)
- [Histórico de Sprints](#-histórico-de-sprints)
- [Definition of Ready (DoR)](#-definition-of-ready-dor)
- [Definition of Done (DoD)](#-definition-of-done-dod)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Modelo de Dados](#modelo-de-dados)
- [Manuais de Instalação e Uso](#-manuais-de-instalação-e-uso)
- [Estratégia de Branching](#-estratégia-de-branching)
- [Padrão de Commit](#-padrão-de-commit)
- [Integrantes do Grupo](#-integrantes-do-grupo)

---

## 📋 Metodologia Utilizada

O framework de Metodologia Ágil utilizado no produto foi o **Scrum**, um método adaptativo, iterativo e eficaz para a gestão de projetos. O trabalho é organizado em Sprints, com cerimônias como Planejamento (Planning), Reuniões Diárias (Dailies) e Revisões (Review) para garantir entregas de valor contínuas e alinhadas às necessidades do cliente.

---

## 🖥️ Tecnologias Utilizadas

Estas foram as tecnologias escolhidas para a produção do projeto:

<div align="center">
  <a href="https://flutter.dev/"><img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white"/></a>
  <a href="https://dart.dev/"><img src="https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white" /></a>
  <a href="https://vuejs.org/"><img src="https://img.shields.io/badge/Vue.js-4FC08D?style=for-the-badge&logo=vue.js&logoColor=white"/></a>
  <a href="https://www.postgresql.org/"><img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/></a>
  <a href="https://git-scm.com/"><img src="https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white"/></a>
  <a href="https://www.java.com/"><img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white"/></a>
  <a href="https://discord.com/"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white"/></a>
  <a href="https://www.atlassian.com/software/jira"><img src="https://img.shields.io/badge/Jira-0052CC?style=for-the-badge&logo=jira&logoColor=white" /></a>
  <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" /></a>


</div>

---

## 📖 Requisitos do Projeto

### Requisitos Funcionais

| Id   | Requisito Funcional                                                                                                                              |
| :--- | :----------------------------------------------------------------------------------------------------------------------------------------------- |
| RF01 | **Gestão de Itens:** Permitir o cadastro, edição e consulta de itens, incluindo nome, unidade de medida e estoque mínimo.               |
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
| RNF07 | **Engenharia do Sistema:** O projeto deve seguir boas práticas de engenharia de software, garantindo modularidade, manutenibilidade e escalabilidade. |

---

| **Rank** | **Prioridade** | **User Story**                                                                                                                                      | **Estimativa** | **Sprint** |
| -------- | -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- | ---------- |
| 1        | Alta           | Como usuário do almoxarifado, quero cadastrar materiais com nome, ficha, grupo, estoque mínimo, unidade, e gerenciar os mesmos                      | 5              | 1          |
| 2        | Alta           | Como gestor, eu quero gerenciar pedidos.                                                                                                            | 5              | 1          |
| 3        | Alta           | Como gestor, quero visualizar os pedidos em aberto.                                                                                                 | 3              | 1          |
| 4        | Alta           | Como gestor da farmácia, quero cadastrar medicamentos com data de validade.                                                                         | 3              | 1          |
| 5        | Alta           | Como usuário, quero fazer login com e-mail e senha.                                                                                                 | 3              | 1          |
| 6        | Alta           | Como usuário, quero acessar os módulos do sistema de acordo com o meu perfil (almoxarifado, farmácia).                                              | 3              | 1          |
| 7        | Alta           | Como usuário, quero acessar a unidade ou estoque na qual eu pertenço.                                                                               | 3              | 1          |
| 8        | Alta           | Como administrador, quero gerenciar usuários (contendo seus perfis na tela de cadastro).                                                            | 5              | 1          |
| 9        | Alta           | Como administrador, quero vincular os usuários a unidades/estoques específicos, garantindo acesso limitado por perfil.                              | 5              | 1          |
| 10       | Alta           | Como administrador, quero cadastrar usuários e fornecedores de forma web.                                                                           | 5              | 1          |
| 11       | Alta           | Como gestor, quero gerenciar fornecedores.                                                                                                          | 3              | 1          |
| 12       | Alta           | Como gestor/administrador, quero cadastrar fornecedores com CNPJ, email e número de empenho.                                                        | 5              | 1          |
| 13       | Alta           | Como gestor/administrador, quero visualizar fornecedores em forma de lista.                                                                         | 3              | 1          |
| 14       | Média          | Como gestor da farmácia, quero cadastrar medicamentos com data de validade.                                                                         | 3              | 1          |
| 15       | Alta           | Como usuário, quero visualizar materiais próximos ou abaixo do estoque mínimo.                                                                      | 3              | 1          |
| 16       | Alta           | Como usuário, quero registrar perdas ou danos em materiais.                                                                                         | 3              | 2          |
| 17       | Média          | Como gestor, quero marcar os pedidos como retirados, contendo a data de retirada.                                                                   | 3              | 2          |
| 18       | Alta           | Como usuário, quero gerar um QR code por material.                                                                                                  | 3              | 2          |
| 19       | Alta           | Como usuário, quero escanear QR code e adicionar a quantidade de novos produtos.                                                                    | 3              | 2          |
| 20       | Alta           | Como gestor, quero visualizar o histórico de pedidos por seção para entender o padrão de consumo.                                                   | 5              | 2          |
| 21       | Alta           | Como usuário, quero ver os materiais mais requisitados por frequência e acompanhar a demanda por meio de gráficos de coluna por grupo de materiais. | 5              | 2          |
| 22       | Alta           | Como gestor, quero ver o status de entrega dos fornecedores e entrega de e-mails enviados.                                                          | 5              | 2          |
| 23       | Alta           | Como gestor, quero disparar e-mails automáticos para fornecedores para evitar atrasos.                                                              | 8              | 2          |
| 24       | Média          | Como usuário, quero visualizar um dashboard com itens em falta/vencimentos.                                                                         | 3              | 2          |
| 25       | Média          | Como usuário, quero visualizar um dashboard com pedidos em aberto.                                                                                  | 3              | 2          |
| 26       | Média          | Como usuário, quero visualizar um dashboard com o consumo mensal por seção.                                                                         | 5              | 2          |
| 27       | Média          | Como usuário, quero receber alertas quando um item estiver próximo do estoque mínimo.                                                               | 5              | 2          |
| 28       | Média          | Como usuário da farmácia/almoxarifado, quero visualizar medicamentos vencidos ou próximos do vencimento.                                            | 3              | 2          |
| 29       | Alta           | Como gestor/administrador, quero cadastrar e gerenciar Seções e associar cada pedido a uma seção para analisar o consumo por seção e geral.         | 5              | 2          |
| 30       | Alta           | Como usuário da farmácia, quero gerir lotes e validades para controlar vencimentos por lote.                                                        | 5              | 2          |
| 31       | Alta           | Como usuário, quero poder prever a quantidade de materiais para o próximo mês através de uma IA.                                                    | 8              | 3          |
| 32       | Alta           | Como gestor, quero gerar relatórios em PDF ou EXCEL incluindo status de estoque (itens em falta, vencimentos).                                      | 5              | 3          |
| 33       | Alta           | Como gestor, quero gerar relatórios em PDF ou EXCEL de pedidos, incluindo em aberto, para conferência com o sistema oficial.                        | 5              | 3          |
| 34       | Média          | Como sistema, quero registrar as ações realizadas pelos usuários, para rastreabilidade.                                                             | 5              | 3          |
| 35       | Média          | Como farmácia, quero poder me comunicar com pacientes para agendamentos e tirar dúvidas.                                                            | 5              | 3          |


---

## Histórico de Sprints

- [**Sprint 1**](docs/sprints/sprint-01.md): Backlog e vídeos de demonstração.
- [**Sprint 2**](docs/sprints/sprint-02.md): Backlog e vídeos de demonstração.

---

## ✅ Backlog da **Sprint 3**
| **Rank** | **Prioridade** | **User Story**                                                                                                                                      | **Estimativa** | **Sprint** |
| -------- | -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- | ---------- |
| 31       | Alta           | Como usuário, quero poder prever a quantidade de materiais para o próximo mês através de uma IA.                                                    | 8              | 3          |
| 32       | Alta           | Como gestor, quero gerar relatórios em PDF ou EXCEL incluindo status de estoque (itens em falta, vencimentos).                                      | 5              | 3          |
| 33       | Alta           | Como gestor, quero gerar relatórios em PDF ou EXCEL de pedidos, incluindo em aberto, para conferência com o sistema oficial.                        | 5              | 3          |
| 34       | Média          | Como sistema, quero registrar as ações realizadas pelos usuários, para rastreabilidade.                                                             | 5              | 3          |
| 35       | Média          | Como farmácia, quero poder me comunicar com pacientes para agendamentos e tirar dúvidas.                                                            | 5              | 3          |
---
## ✅ Definition of Ready (DoR)
Critérios de aceitação para assegurar a qualidade de uma issue:
[📄 Definition of Ready (DoR) — docs/dor.md](docs/dor.md)

---

## ✅ Definition of Done (DoD)
Critérios de aceitação e qualidade para encerrar uma issue/PR:  
[📄 Definition of Done (DoD) — docs/dod.md](docs/dod.md)

---

## 📂 Estrutura do Projeto

![Estrutura do Projeto](docs/diagrams/structure.jpg)

---

## Modelo de Dados

Modelo inicial (Entidades, atributos e relacionamentos).

![Modelo de Dados](docs/diagrams/modeloDeDados.png)

---

## 📚 Manuais de Instalação e Uso

- **ManagementService**
  - [Manual de Instalação](https://github.com/Code-Nine-FTC/ManagementService/blob/main/docs/manual-de-instalacao.md)
  - [Manual do Usuário](https://github.com/Code-Nine-FTC/ManagementService/blob/main/docs/manual-do-usuario.md)
- **MobileInterface-2025.2**
  - [Manual de Instalação](https://github.com/Code-Nine-FTC/MobileInterface-2025.2/blob/main/docs/manual-de-instalacao.md)
  - [Manual do Usuário](https://github.com/Code-Nine-FTC/MobileInterface-2025.2/blob/main/docs/manual-do-usuario.md)
- **WebInterface-2025.2**
  - [Manual de Instalação](https://github.com/Code-Nine-FTC/WebInterface-2025.2/blob/main/docs/manual-de-instalacao.md)
  - [Manual do Usuário](https://github.com/Code-Nine-FTC/WebInterface-2025.2/blob/main/docs/manual-do-usuario.md)

---

## 🌿 Estratégia de Branching

A estratégia de branching define como o código é gerenciado no Git. Para detalhes completos, consulte o documento:  
[📄 Estratégia de Branching — docs/estrategia-de-branch.md](docs/estrategia-de-branch.md)

---

## ✨ Padrão de Commit

O padrão de commit garante mensagens claras e consistentes no histórico do projeto. Para detalhes, consulte o documento:  
[📄 Padrão de Commit — docs/padrao-de-commits.md](docs/padrao-de-commits.md)

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
