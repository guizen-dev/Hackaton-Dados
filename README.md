# 🧠 Hackathon de Geodados e Ingresso na UFABC – Planejamento

## 📅 Carga horária recomendada por pessoa

| Semana       | Sprint                          | Carga total estimada (equipe) | Carga por pessoa (4 integrantes) |
|--------------|----------------------------------|-------------------------------|----------------------------------|
| 19–25/05     | Sprint 1 – Coleta e Limpeza     | 24 horas                      | 6h                               |
| 26/05–01/06  | Sprint 2 – Análise Exploratória | 32 horas                      | 8h                               |
| 02–08/06     | Sprint 3 – Hipóteses e Modelos  | 32 horas                      | 8h                               |
| 09–12/06     | Sprint 4/5 – Finalização        | 32 horas                      | 8h                               |

**Total recomendado por pessoa:** ~30 horas no projeto (7 a 8 horas por semana)

---

## 🟦 Sprint 1 – Coleta e limpeza de dados
📆 **Período:** 19 a 25 de maio  
🎯 **Objetivo:** Obter todas as bases, limpar nomes de regiões e padronizar formatos  

### 🔹 Tarefas por pessoa

**👤 Pessoa 1 – Gestor de dados**
- [ ] Baixar base do SISU da UFABC (nome, curso, nota, município)
- [ ] Padronizar nomes de municípios (sem acento, siglas, etc)
- [ ] Criar dicionário de dados `documentacao/dicionario_bases.md`

**👤 Pessoa 2 – Geodados**
- [ ] Baixar shapefiles dos bairros de SP, Santo André, São Bernardo
- [ ] Baixar linhas de ônibus, metrô e trem (GeoSampa / SIGA)
- [ ] Testar visualizações no QGIS ou Kepler.gl

**👤 Pessoa 3 – ENEM / Ensino Médio**
- [ ] Baixar microdados ENEM e Censo Escolar (2022–2023)
- [ ] Criar amostra da região do ABC
- [ ] Padronizar colunas principais: nota, escola, localização

**👤 Pessoa 4 – Mobilidade e Desigualdade**
- [ ] Baixar dados do IBGE: população jovem, renda, escolaridade
- [ ] Criar base por bairro/município com essas variáveis

---

## 🟩 Sprint 2 – Análise exploratória e cruzamentos iniciais
📆 **Período:** 26 de maio a 01 de junho  
🎯 **Objetivo:** Explorar padrões geográficos e desigualdades no ingresso

### 🔹 Tarefas (todos)

- [ ] Criar mapas de calor dos ingressantes por cidade e bairro
- [ ] Calcular densidade de ingressantes por mil jovens (15–19 anos)
- [ ] Cruzar nota média do ENEM por região com taxa de ingresso
- [ ] Mapear regiões com boas escolas mas poucos ingressantes
- [ ] Identificar regiões com 2+ conduções ou tempo de deslocamento alto

📍 **Ao fim da sprint:** Reunião para decidir foco do projeto (transporte, desigualdade, tipo de escola)

---

## 🟨 Sprint 3 – Hipóteses e modelagem
📆 **Período:** 02 a 08 de junho  
🎯 **Objetivo:** Testar hipóteses, criar métricas comparáveis e rascunhar visualizações

### 🔹 Tarefas

- [ ] Criar métricas comparáveis:
  - Ingressantes por 10 mil jovens
  - % de alunos por tipo de escola por região
  - Distância média entre casa e UFABC
- [ ] Testar hipóteses:
  - Proximidade x ingresso
  - Transporte público x ingresso
  - Alta nota + distância = desistência?
- [ ] Iniciar gráficos e painéis interativos (Plotly, Dash, Power BI)

---

## 🟥 Sprint 4/5 – Consolidação e entrega final
📆 **Período:** 09 a 12 de junho  
🎯 **Objetivo:** Finalizar painéis, relatório e apresentação

### 🔹 Tarefas finais

- [ ] Gerar mapas finais com overlays (transporte + escolas + ingresso)
- [ ] Escrever resumo com hipóteses, achados e políticas públicas sugeridas
- [ ] Montar painel com filtros (região, tipo de escola, transporte)
- [ ] Limpar notebooks e gerar prints ou HTML
- [ ] Criar backup dos dados organizados

---

🧩 **Observação:** O tema pode ser redirecionado conforme os achados da Sprint 2  
💡 **Dica:** Centralizar bases e insights num repositório compartilhado (GitHub ou GDrive estruturado) com um catálogo de dados

