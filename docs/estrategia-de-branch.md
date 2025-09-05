# Estratégia de Branching

## Fluxo adotado: Git Flow

**Principais branches:**
- `main`: código estável em produção  
- `develop`: integração contínua de features  
- `feature/*`, `release/*`, `hotfix/*`: isolam alterações por tipo de trabalho

**Vantagens:**
- Organização clara entre desenvolvimento e produção  
- Suporte a versões múltiplas via branches de release

**Conveniência de nomes**

| Tipo     | Prefixo         | Exemplo                  |
|----------|------------------|--------------------------|
| Feature  | `feature/`       | `feature/login-api`      |
| Hotfix   | `hotfix/`        | `hotfix/login-error`     |
| Release  | `release/`       | `release/v1.0.0`         |
| Docs     | `docs/`          | `docs/update-readme`     |

**Fluxo resumido:**
feature/* → (PR) → develop → release/* → (PR) → main → tag → hotfix/*