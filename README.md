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

## 👤 Pessoa 1 – Gestor de Dados + Infra de Arquivos
🕒 ~6h
- [ ] Baixar base do SISU completa (ZIP), mas extrair e filtrar só SP ou ABC  
- [ ] Padronizar nomes de municípios (acentos, siglas etc)  
- [ ] Estruturar Google Drive com:  
  - `/raw/` para arquivos originais  
  - `/sample/` para amostras leves  
  - `/processed/` para saídas intermediárias  
- [ ] Subir amostras para o Drive
- [ ] Criar notebook exemplo de leitura e limpeza da amostra SISU  

---

## 👤 Pessoa 2 – Geodados + Mapas Base
🕒 ~6h
- [ ] Baixar shapefiles de SP, Santo André, São Bernardo  
- [ ] Baixar dados de transporte (ônibus, metrô, trem - GeoSampa/SIGA)  
- [ ] Criar mapa base em QGIS ou Kepler.gl com:  
  - Bairros + UFABC + Linhas de transporte  
- [ ] Exportar `.geojson` ou `.png` com preview do mapa  
- [ ] Subir para o Drive na pasta `/mapas_base/` com legenda + fontes  

---

## 👤 Pessoa 3 – ENEM e Censo Escolar
🕒 ~6h
- [ ] Baixar microdados do ENEM (apenas SP ou ABC)  
- [ ] Criar amostra reduzida (com 1–2% dos dados ou só do ABC)  
- [ ] Padronizar colunas principais: nota, tipo de escola, localização  
- [ ] Baixar dados do Censo Escolar 2022–2023  
- [ ] Identificar escolas com maior nº de participantes do ENEM  
- [ ] Subir amostras para o Drive + salvar dicionário de colunas usadas  

---

## 👤 Pessoa 4 – IBGE + Indicadores Sociais
🕒 ~6h
- [ ] Baixar dados do IBGE:  
  - População jovem (15–19)  
  - Renda média  
  - Escolaridade  
- [ ] Cruzar dados por bairro ou município (usar códigos IBGE)  
- [ ] Criar CSV leve com indicadores por região (ABC/SP)  
- [ ] Subir base no Drive + documentar origem e granularidade  

📌 **Resultado esperado da Sprint 1:**
- Bases brutas coletadas e parcialmente tratadas
- Estrutura de pastas padronizada
- Nomes de cidades e regiões normalizados
- Dicionário de dados iniciado
- Primeiros mapas de teste com regiões e transporte

----

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

