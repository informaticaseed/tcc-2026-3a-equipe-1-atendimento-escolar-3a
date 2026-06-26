# Arquitetura do Sistema

**Grupo:** Equipe 01 
**Última atualização:** 26/06/2026

---

## Diagrama de arquitetura

```
Usuário (Aluno ou Direção)
↓
[Tela HTML — templates/]
↓
[app.py — rotas Flask]
↓
[repositorio.py — acesso ao banco]
↓
[banco.db — SQLite]

```
---

## Separação de camadas

| Camada | Arquivo | Responsabilidade |
|--------|---------|-----------------|
| Web | `src/app.py` | Rotas, controle de endpoints e renderização de telas |
| Dados | `src/repositorio.py` | Toda a execução SQL, consultas e persistência via SQLAlchemy |
| Templates | `src/templates/` | Renderização do HTML dinâmico ao usuário final |
| Testes | `tests/` | Validações automáticas do ciclo do software |

---

## Decisões técnicas

Ver pasta `docs/decisoes/` para os registros de decisão técnica (ADR).
