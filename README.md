# TCC 2026 — [Nome do Grupo]
**LTP3 + QP3 · CEMIC 2026 · Prof. Rafael Martins Alves**

---

## 👥 Integrantes

| Nome completo          | GitHub    | Turma |
|------------------------|-----------|-------|
| Alessa | @username | 3A |
| Caio Vitor | @username | 3A |
| Daniel Alves| @username | 3A |
| Guilherme de Sousa Paz | @GuilhermeSPaz18 | 3A |
| Sara Texeira | @username | 3A |

**Tema:** Portal de Atendimento, Suporte e Ouvidoria Interna para os estudantes e servidores do CEMI.
**Tecnologia:** Python + Flask + SQLite

---

## 🎯 O que o sistema faz

O sistema centraliza e organiza a comunicação interna do CEMI, permitindo que estudantes abram chamados, tirem dúvidas e enviem sugestões diretamente para a administração da escola através de uma interface web com chat contínuo. Ele resolve o problema de solicitações perdidas ou demoradas em canais informais, oferecendo um painel administrativo para a gestão de pendências e controle de níveis de acesso (Alunos e Atendentes/ADM).

---

## 🔄 Como o grupo trabalha toda semana

1. **Segunda** — cada integrante abre Issues da semana (use o template "Tarefa Semanal")
2. **Durante a semana** — trabalham e fazem commits
3. **Sexta** — o grupo abre 1 Pull Request linkando as Issues concluídas
4. **Push** — métricas de participação aparecem automaticamente no Actions

---

## 📁 Estrutura do projeto

```
├── README.md           ← O arquivo principal (com o grupo e o tema)
├── BACKLOG.md          ← Onde vamos listar as funcionalidades
├── src/                ← TODO O CÓDIGO FONTE DO SITE FICA AQUI
│   ├── app.py          ← Arquivo principal que roda o Flask
│   ├── database.db     ← O banco de dados SQLite
│   ├── templates/      ← Seus arquivos HTML (login, index, chat, adm)
│   └── static/         ← Seus arquivos CSS, JS e Imagens do layout
├── docs/               ← Relatórios, diagramas e decisões técnicas
├── diagramas/          ← Imagem da arquitetura do sistema
├── evidencias/         ← Prints da tela do site funcionando
└── tests/              ← Testes automatizados do sistema
```

---

## ⚡ Comandos rápidos

```bash
# Clonar o repositório
git clone <URL>

# Rodar o projeto
pip install -r requirements.txt
python src/app.py

# Rodar os testes
pytest tests/ -v
