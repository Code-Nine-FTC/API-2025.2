# Definition of Done (DoD)

**Objetivo:** Estabelecer um padrão de qualidade compartilhado que uma entrega (issue/PR) deve atender para ser considerada concluída. O DoD garante que o trabalho é funcional, testado, documentado e pronto para ser integrado.

---

### Checklist de Conclusão

Uma issue é considerada **Done** quando o Pull Request (PR) associado cumpre os seguintes critérios:

#### 1. Código e Desenvolvimento
-   **[ ] Código Funcional:** A implementação atende a todos os critérios de aceitação definidos na issue.
-   **[ ] Padrões de Código:** O código segue os guias de estilo e padrões do projeto (linting sem erros).
-   **[ ] Branching Correto:** O código está em uma branch apropriada (`feature/*`, `hotfix/*`) e o PR direciona para a branch correta (`develop`, `homolog` ou `main`).

#### 2. Testes e Qualidade
-   **[ ] Testes Unitários:** Novos testes unitários foram criados para a lógica implementada e os testes existentes continuam passando.
-   **[ ] Cobertura de Teste:** A cobertura de testes se mantém ou aumenta, conforme o padrão definido pela equipe.
-   **[ ] Teste Manual Validado:** A funcionalidade foi validada manualmente em ambiente de desenvolvimento ou staging.

#### 3. Revisão e Integração
-   **[ ] Pull Request (PR) Bem Descrito:** O PR possui um título claro, uma descrição do que foi feito e o link para a issue correspondente.
-   **[ ] Code Review Aprovado:** O código foi revisado e aprovado por, no mínimo, um outro membro da equipe.

#### 4. Documentação
-   **[ ] Documentação Técnica Atualizada:** Se aplicável, a documentação de APIs (ex: Swagger), READMEs de serviços ou manuais foram atualizados.

---

**Nota:** Apenas após o cumprimento de todos os itens do DoD e o merge do PR, a issue pode ser movida para a coluna "Done".
