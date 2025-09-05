# Definition of Done (DoD) — Versão Inicial

**Objetivo:** Critérios mínimos que uma issue/PR deve cumprir para ser considerada concluída.

## Critérios obrigatórios
- [ ] Código commitado em branch feature/* ou hotfix/*.
- [ ] Pull Request criado com descrição, issue vinculada e checklist DoD preenchido.
- [ ] Linter e checks estáticos (ESLint/Flake8) sem erros.
- [ ] Testes automáticos relevantes adicionados/atualizados e rodando com status OK.
- [ ] Cobertura mínima acordada para módulos críticos (definir por equipe).
- [ ] Revisão aprovada (mínimo 1 reviewer) e CI verde.
- [ ] Documentação atualizada: README do serviço / endpoint / passos de deploy quando aplicável.
- [ ] Migrações (se houve alteração no DB) criadas e testadas localmente.
- [ ] Demonstração manual ou evidência (print, vídeo curto ou link para demo) disponível se funcionalidade afetar fluxo do usuário.
- [ ] Merge via PR (sem fast-forward direto em main/protected branches).

## Critérios de qualidade (quando aplicável)
- [ ] Tratamento de erros e logs adequados.
- [ ] Validações de input/segurança implementadas.
- [ ] Dependências externas avaliadas (privacidade/permissões da câmera, etc).

---

**Notas**
- Itens adicionais podem ser exigidos por sprint (ex.: revisão de arquitetura, auditoria de segurança).
- Time pode elevar requisitos (ex.: nº mínimo de reviewers, cobertura de testes) por consenso.