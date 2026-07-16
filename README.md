# 📊 QA Processos

- Processos, artefatos e documentação da equipe de Qualidade – priorização de automação, testes exploratórios, RCAs e relatórios.

## 📌 Sobre o Repositório

Este repositório centraliza todos os **processos, artefatos e documentação** criados por mim . Ele foi criado para:

- ✅ Padronizar a gestão de testes e automação
- ✅ Versionar planilhas e documentos importantes
- ✅ Registrar análises de causa raiz e melhorias

----------
## 📁 Estrutura de Pastas

qa-processos/
│
├── 01-gestao-testes/
│ ├── matriz-priorizacao/ # Planilha de priorização de automação
│ │ ├── Matriz_Priorizacao_Automacao_v1.0.xlsx
│ │ └── LEIA-ME.md # Como usar a matriz
│ │
│ └── exploratorios/ # Relatórios de testes exploratórios
│ ├── sessoes/ # Relatórios por sprint/release
│ ├── templates/ # Template para novos exploratórios
│ ├── evidencias/ # Prints e vídeos organizados
│ └── LEIA-ME.md # Como documentar exploratórios
│
├── 02-processos-melhoria/
│ └── rcas-e-acoes/ # Análises de causa raiz
│ ├── modelo-analise-causa-raiz.docx
│ └── LEIA-ME.md # Como preencher um RCA

├── docs/ # Documentação geral
│ ├── padrao-nomenclatura.md # Regras de nomenclatura
│ └── onboarding-qa.md # Guia para novos QAs (opcional)
│
├── README.md # Este arquivo
└── .gitignore # Arquivos ignorados pelo Git


---

## ✅ Boas Práticas

### 📝 Commits
Use mensagens claras e padronizadas:

| Tipo | Exemplo |
|------|---------|
| `feat:` | `feat: adiciona novo candidato à automação` |
| `docs:` | `docs: atualiza guia de testes exploratórios` |
| `fix:` | `fix: corrige fórmula na planilha de priorização` |
| `refactor:` | `refactor: reorganiza estrutura de pastas` |

### 📂 Versionamento de Arquivos
- Arquivos principais (planilhas, templates) devem usar **versionamento semântico**:
  - `v1.0` → Primeira versão estável
  - `v1.1` → Pequenas alterações
  - `v2.0` → Mudanças significativas

- **Nunca** sobrescreva um arquivo versionado sem criar uma nova versão.

## 🤝 Como Contribuir

1. **Clone** o repositório
   ```bash
   git clone https://github.com/seu-usuario/qa-processos.git

git checkout -b feat/minha-melhoria
git add .
git commit -m "feat: adiciona novo template de exploratório"
git push origin feat/minha-melhoria



