
# Objetivo
A Matriz de Priorização de Automação tem como objetivo auxiliar o time de QA a tomar decisões baseadas em dados sobre quais testes automatizar primeiro, considerando critérios objetivos como:

Frequência de execução

Estabilidade da funcionalidade

Risco de negócio

Nível de julgamento humano necessário

Tempo gasto na execução manual

Volume de dados e variações de teste

O resultado é uma recomendação clara (Prioridade Alta, Com Cuidado, Avaliar ou Não Automatizar) que permite ao time priorizar o backlog de automação de forma estruturada e transparente.

Como preencher

# Passo 1: Acesse a aba correta

Abra a planilha qa_automacao_seguros.xlsx e vá para a aba "Candidatos à Automação".

# Passo 2: Identifique um candidato

Para cada fluxo ou caso de teste que você considera candidato à automação, preencha uma nova linha com as seguintes informações:

Coluna	O que preencher	

Exemplo

### Passo 2: Identifique um candidato

Para cada fluxo ou caso de teste que você considera candidato à automação, **preencha uma nova linha** com as seguintes informações:

### Passo 2: Identifique e documente o candidato

Preencha as colunas de identificação do teste. As colunas em **negrito** são obrigatórias:

| Coluna | Tipo | Descrição | Exemplo |
|--------|------|-----------|---------|
| **#** | Automático | Número sequencial da linha | 11 |
| **Nome do Teste / Fluxo** | Texto | Nome descritivo do fluxo | "Recálculo de prêmio após endosso" |
| **Módulo / Área** | Texto | Área do sistema | Emissão |
| **Sprint / Data** | Texto | Sprint ou data da análise | Sprint 5 |
| **Frequência** | Número (0-3) | Nota para frequência de execução | 3 |
| **Estabilidade** | Número (0-3) | Nota para estabilidade da funcionalidade | 2 |
| **Risco de Negócio** | Número (0-3) | Nota para risco de negócio | 3 |
| **Julgamento Humano** | Número (0-3) | Nota para necessidade de julgamento humano | 3 |
| **Tempo Manual** | Número (0-3) | Nota para tempo de execução manual | 2 |
| **Volume de Dados** | Número (0-3) | Nota para volume de dados e variações | 3 |
| **Pontuação Total** | Automático | Soma das notas (calculada pelo Excel) | 16 |
| **Recomendação** | Automático | Classificação baseada na pontuação | AUTOMATIZE COM PRIORIDADE |
| **Responsável QA** | Texto | Quem está analisando o teste | @seu-usuario |
| **Observações** | Texto | Comentários adicionais | "Fluxo crítico para o negócio" |


# Passo 3: Atribua notas para cada critério
Para cada um dos 6 critérios, atribua uma nota de 0 a 3 conforme a tabela abaixo:

## Critérios de Avaliação (nota de 0 a 3)

| Critério | Nota 0 | Nota 1 | Nota 2 | Nota 3 |
|----------|--------|--------|--------|--------|
| **Frequência** | Raro / pontual | Mensal | Semanal / por sprint | Diária / por build |
| **Estabilidade** | Muda toda sprint | Muda às vezes | Raramente muda | Estável / legado |
| **Risco de Negócio** | Baixo impacto | Impacto moderado | Alto impacto | Crítico (financeiro/regulatório) |
| **Julgamento Humano** | Alta subjetividade | Alguma análise visual | Resultado claro mas visual | 100% objetivo |
| **Tempo Manual** | Menos de 2 min | 2 a 10 min | 10 a 30 min | Mais de 30 min |
| **Volume de Dados** | Um único cenário | Poucos casos | Muitos casos | Data-driven / massivo |

---

## Escala de Recomendação

| Pontuação | Recomendação |
|-----------|--------------|
| **14 – 18** |  AUTOMATIZE COM PRIORIDADE |
| **10 – 13** |  AUTOMATIZE COM CUIDADO |
| **5 – 9** |  AVALIE ANTES DE AUTOMATIZAR |
| **0 – 4** |  NÃO AUTOMATIZE AGORA |

# Passo 4: Leia o resultado
As colunas "Pontuação Total" e "Recomendação" são calculadas automaticamente pelo Excel. Você não precisa fazer nenhuma fórmula.

## Resultado (calculado automaticamente)

| Coluna | O que mostra |
|--------|--------------|
| **Pontuação Total** | Soma de todas as notas (máximo de 18 pontos) |
| **Recomendação** | Classificação automática baseada na pontuação |

# Passo 5: Acompanhe no Dashboard

A aba "Dashboard" atualiza automaticamente com:

Total de candidatos avaliados

Distribuição por faixa de prioridade

Top candidatos para automação

