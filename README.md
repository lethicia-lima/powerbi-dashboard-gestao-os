# 📈 Dashboard de Gestão e Performance de Ordens de Serviço (OS) no Power BI

---

## 🎯 Visão Geral e Problema de Negócio

Este projeto envolve o desenvolvimento completo de um painel de Business Intelligence (BI) para a gestão de Ordens de Serviço.

O objetivo foi fornecer à equipe gerencial uma visão **clara e acionável** para monitorar o **volume de trabalho**, a **conformidade com prazos (SLA)** e a **distribuição de recursos** com base nos tipos de serviço.

**Valor Demonstração:** Proficiência em Power BI (DAX, Power Query), Modelagem de Dados e tradução de métricas de negócio em KPIs visuais.

## 🔑 Indicadores Chave de Performance (KPIs)

O dashboard foi projetado para responder a perguntas críticas, utilizando os seguintes indicadores:

| Área de Análise | Indicador Principal | Métrica no Dashboard |
| :--- | :--- | :--- |
| **Volume de Trabalho** | Tendência de Abertura de OS | Contagem de Ordens de Serviço ao longo do tempo. |
| **Conformidade** | Atraso no Atendimento (SLA) | Quantidade de OS em Atraso por faixas de tempo. |
| **Carga de Trabalho** | Distribuição de Serviços | Análise de Pareto (80/20) dos 'Tipos de OS'. |

## 📊 Estrutura do Dashboard e Visualizações

### 1. Análise Temporal e Tendências

* **Gráficos:** Linhas e Colunas.
* **Função:** Identificar picos sazonais (mensais) e tendências de longo prazo na criação de OS, ajudando a planejar a capacidade da equipe.

### 2. Análise de Desempenho (SLA)

* **Gráficos:** Cartões (KPI Principal), Colunas Clusterizadas.
* **Método:** Uso de uma medida **DAX** para calcular a diferença de dias e classificar o status como "Em Atraso" ou "No Prazo", segmentando o problema por faixas de atraso (ex: 1-3 dias).

### 3. Distribuição de Carga de Trabalho

* **Gráficos:** Barras Horizontais (Top N) e Rosca.
* **Função:** Mostrar visualmente quais **Tipos de OS** representam a maior parte do volume de trabalho, direcionando a alocação de recursos (Princípio de Pareto).

## 🛠️ Destaques Técnicos e Modelagem

* **Power Query (Linguagem M):** Utilizado para a etapa de **ETL (Extração, Transformação e Carga)**, incluindo a criação de **Colunas Condicionais** para classificação de status e **Mesclagem de Consultas (Merge Queries)** para enriquecimento de dados de múltiplas fontes.
* **Modelagem:** Implementação de um esquema dimensional otimizado, garantindo relacionamentos 1:N entre tabelas de Fato (OS) e tabelas de Dimensão (Tipos de Serviço, Colaboradores).

## Visualização

<img width="1150" height="656" alt="image" src="https://github.com/user-attachments/assets/f39c336d-89ab-45fd-b937-f9a942d5ba6f" />

**➡️ [Acesse o Painel Interativo AQUI](DASHBOARD.pbix)**

**➡️ [Acesse o Dicionário de Dados completo AQUI](dicionariodedados.xlsx)**
