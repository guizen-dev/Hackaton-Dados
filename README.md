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

## 👤 Pessoa 1 – Gestor de Dados + Apoio ao ENEM
🕒 ~6h
- [ ] Baixar base do SISU (nome, curso, nota, município), extrair e filtrar só SP ou ABC (apoio à pessoa 3)
- [ ] Padronizar nomes de municípios (sem acento, siglas, etc)
- [ ] Estruturar Google Drive com:  
  - `/raw/` para arquivos originais  
  - `/sample/` para amostras leves  
  - `/processed/` para saídas intermediárias  
- [ ] Subir amostras para o Drive
- [ ] Criar notebook exemplo de leitura e limpeza da amostra SISU  

---

## 👤 Pessoa 2 – Geodados + Apoio a Mobilidade  
🕒 ~6h
- [ ] Baixar shapefiles de SP, Santo André, São Bernardo  
- [ ] Baixar dados de transporte (ônibus, metrô, trem - GeoSampa/SIGA)  
- [ ] Identificar variáveis geográficas para cruzamento (nome do bairro, ID, coordenadas)  
- [ ] Baixar e organizar camadas base (vias, transporte público, linhas férreas etc)  
- [ ] Criar preview de mapa base com bairros + infraestrutura de transporte
  - Bairros + UFABC + Linhas de transporte  
- [ ] Subir para o Drive na pasta `/mapas_base/` com legenda + fontes  

---

## 👤 Pessoa 3 – ENEM / Ensino Médio 
🕒 ~6h
- [ ] Filtrar candidatos da região do ABC nos microdados do ENEM (com apoio da Pessoa 1)  
- [ ] Padronizar colunas principais: nota, tipo de escola, localização
- [ ] Cruzar município de residência com codificação dos dados do ENEM  
- [ ] Baixar e filtrar dados do Censo Escolar (2022–2023) para escolas do ABC  
- [ ] Identificar escolas com maior número de participantes do ENEM
- [ ] Subir amostras para o Drive + salvar dicionário de colunas usadas  

---

### 👤 Pessoa 4 – Mobilidade e Desigualdade  
🕒 Carga estimada: ~6h  
- [ ] Baixar dados do IBGE:  
  - População jovem (15–19 anos)  
  - Renda média domiciliar  
  - Escolaridade média  
- [ ] Agregar os dados por bairro/município (usar pandas ou QGIS)  
- [ ] Iniciar base estruturada com variáveis socioeconômicas por região  
- [ ] Verificar compatibilidade entre dados do IBGE e shapefiles (IDs, nomes)

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

