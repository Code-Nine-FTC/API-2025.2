# Estratégia de Branching

## Fluxo Adotado

O projeto utiliza um fluxo baseado no Git Flow, com a adição de uma branch para homologação, garantindo um processo de validação antes da produção.

### Branches Principais

Estas são as branches que existirão durante todo o ciclo de vida do projeto:

-   `main`: Contém o código estável que está em produção. Todo commit nesta branch deve ser uma versão funcional e testada, pronta para ser entregue aos usuários.
-   `homolog`: Ambiente de pré-produção. Recebe o conteúdo da `develop` para a realização de testes de aceitação e validação. É a última etapa antes do código ir para a `main`.
-   `develop`: Branch de integração contínua. Centraliza o desenvolvimento de novas features e correções que farão parte da próxima versão.

### Branches de Suporte

Estas branches são temporárias e servem para isolar o trabalho em andamento:

-   `feature/*`: Utilizada para o desenvolvimento de novas funcionalidades. É criada a partir da `develop`.
-   `hotfix/*`: Destinada a correções urgentes em produção.
-   `docs/*`: Usada para alterações e atualizações na documentação.

### Convenções de Nomenclatura

| Tipo de Trabalho | Prefixo         | Exemplo de Branch        |
| ---------------- | --------------- | ------------------------ |
| Feature          | `feature/`      | `feature/nova-api-login` |
| Hotfix           | `hotfix/`       | `hotfix/erro-login-500`  |
| Documentação     | `docs/`         | `docs/atualizar-readme`  |

### Fluxo de Desenvolvimento

1.  **Desenvolvimento de Features**:
    -   O desenvolvedor cria uma nova branch `feature/*` a partir da `develop`.
    -   Após a conclusão, abre um Pull Request (PR) da `feature/*` para a `develop`.

2.  **Processo de Homologação**:
    -   Quando um conjunto de features está pronto para ser testado, o conteúdo da `develop` é mesclado na branch `homolog` através de um PR.
    -   A equipe realiza os testes de validação no ambiente de homologação.

3.  **Lançamento em Produção**:
    -   Após a aprovação em homologação, o conteúdo da `homolog` é mesclado na `main` através de um PR.

4.  **Correções Urgentes (Hotfix)**:
    -   Uma branch `hotfix/*` é criada a partir da `main`.
    -   Após a correção, a branch é mesclada de volta na `main` e também em `homolog` e `develop` para garantir que a correção seja incorporada em todas as frentes de trabalho.

Ao final, as branches `develop`, `homolog` e `main` permanecem, refletindo os diferentes estágios do ciclo de vida do software.
