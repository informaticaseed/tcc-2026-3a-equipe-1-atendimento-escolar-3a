# ADR 001 — Escolha da Stack Tecnológica do MVP

**Data:** 26/06/2026
**Status:** Aceita

---

## Contexto

O projeto exige o desenvolvimento ágil de uma ferramenta de ouvidoria segura para mitigar problemas de comunicação interna no ambiente escolar. Era necessário um ecossistema leve, que operasse eficientemente em ambientes de desenvolvimento locais com restrições de hardware e oferecesse mecanismos nativos rápidos de persistência e session management.

---

## Alternativas consideradas

- **Opção A: Node.js + Express + PostgreSQL** 
  - Vantagem: Alta performance com I/O assíncrono.
  - Desvantagem: Maior verbosidade para configurar e overhead desnecessário de gerenciamento de servidores de banco externos para o escopo inicial do MVP.
- **Opção B: Python + Flask + SQLite**
  - Vantagem: Curva de aprendizado rápida, sintaxe limpa, microrframework extremamente flexível e banco baseado em um único arquivo local extremamente portátil.
  - Desvantagem: Não recomendado para aplicações de altíssima escala simultânea (fora do escopo da comunidade local do CEMI).

---

## Decisão

O grupo optou pela **Opção B (Python + Flask + SQLite)**. A escolha foi motivada pela modularidade do Flask, que permite integrar facilmente o SQLAlchemy para a modelagem relacional de chamados e denúncias sem adicionar complexidade na infraestrutura local de teste dos desenvolvedores.

---

## Consequências

O desenvolvimento do backend torna-se centralizado no diretório `src/`, utilizando o arquivo `app.py` como núcleo gerenciador de rotas e o arquivo `repositorio.py` para isolar todas as interações de escrita e leitura de dados pedagógicos.
