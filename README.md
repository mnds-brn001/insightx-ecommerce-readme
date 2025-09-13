<!-- 
*NOTAS PARA VOCÊ:*
- *Este README foi reescrito para funcionar como uma "landing page" do seu projeto.* 
- *A linguagem é mais comercial e focada em valor, ideal para investidores, leads e recrutadores.*
- *Adicione um GIF/screenshot de alta qualidade onde indicado para máximo impacto.*
- *Links para o "Live Demo" devem ser atualizados quando disponíveis.*
-->

<div align="center">

# Insight Expert · E-commerce Analytics Dashboard

### **Transformando dados brutos de e-commerce em inteligência acionável.**

<p>
    <img src="https://img.shields.io/badge/Python-3.11+-blue.svg" alt="Python 3.11+">
    <img src="https://img.shields.io/badge/Streamlit-1.34+-red.svg" alt="Streamlit">
    <img src="https://img.shields.io/badge/Pandas-2.2+-purple.svg" alt="Pandas">
    <img src="https://img.shields.io/badge/Plotly-5.22+-3975E5.svg" alt="Plotly">
    <img src="https://img.shields.io/badge/Scikit--learn-1.5+-F8991D.svg" alt="Scikit-learn">
    <img src="https://img.shields.io/badge/license-Proprietary-important.svg" alt="Proprietary License">
</p>
</div>

---

<!-- 
==================================================================================================================================
ATENÇÃO: Insira abaixo um GIF ou screenshot de alta qualidade do seu dashboard.
Exemplo: ![InsightX Dashboard](URL_DO_SEU_GIF_OU_IMAGEM.gif)
==================================================================================================================================
-->

<br>

## 1. A Vantagem Insight Expert: De Dados a Decisões Estratégicas

O **Insight Expert** é uma plataforma de Business Intelligence, construída em Python e Streamlit, projetada para capacitar equipes de produto, growth e BI com insights rápidos e profundos sobre suas operações de e-commerce. Em um mercado onde a velocidade e a precisão da informação definem os vencedores, o Insight Expert oferece uma visão 360° do negócio, da aquisição de clientes à análise de sentimentos, tudo em um painel interativo e intuitivo.

Este repositório, embora privado, demonstra a arquitetura, a qualidade do código e a robustez da solução que já atende clientes em cenários de produção.

---

## 2. Resolvendo Desafios Reais do E-commerce

Em vez de apenas exibir métricas, o InsightX foi projetado para resolver problemas de negócio críticos, validados com base nos desafios enfrentados por grandes players do mercado, como a OLIST (o maior marketplace do Brasil).

| Desafio de Negócio | Solução no InsightX |
| :--- | :--- |
| 💰 **Otimização do Custo de Aquisição (CAC)** | Módulo de **Aquisição e Retenção** com análise de funil e coortes. |
| 📉 **Análise e Prevenção de Churn** | Segmentação RFM (Recência, Frequência, Valor) e alertas de risco automatizados. |
| 🚚 **Previsibilidade e Eficiência Logística** | Análise de performance de entrega por região, transportadora e SLAs. |
| 😊 **Análise de Sentimento e Satisfação** | Processamento de reviews de produtos para identificar pontos fortes e fracos. |
| 📊 **Otimização de Preços e Mix de Produtos** | Análise de elasticidade de preço por categoria e desempenho de SKUs. |
| 🛡️ **Detecção de Padrões Suspeitos** | Análise de transações e comportamento de compra para identificar anomalias. |

---

## 3. Funcionalidades em Destaque

- **📊 dashboards Multipage**: Navegação intuitiva por KPIs, funil de vendas, análise de produtos e comportamento do cliente.
- **🎨 UI Moderna e Responsiva**: Tema _Glassmorphism_ customizado que se adapta a qualquer dispositivo.
- **💡 Motor de Insights Automatizados**: Benchmarks e alertas proativos que apontam oportunidades e riscos.
- **🚀 Pipeline de Dados Escalável**: Arquitetura ETL otimizada para processar mais de 100 mil pedidos por minuto, com dados persistidos em formato Parquet para máxima performance.
- **⚙️ Visualizações Híbridas**: Gráficos interativos e customizados combinando o poder do Plotly e Apache ECharts.
- **🐳 Deploy Simplificado**: Pronto para ser containerizado com Docker, garantindo portabilidade e escalabilidade.

---

## 4. Arquitetura e Stack Tecnológica

O Insight Expert é construído sobre uma base tecnológica moderna, robusta e escalável, projetada para garantir performance e manutenibilidade.

### Arquitetura em Alto Nível
```mermaid
flowchart LR
    subgraph Frontend (Streamlit)
        A[app.py › Roteamento]
        B[paginas/*.py]
        C[components/*]
    end
    subgraph Core
        D[utils/ — KPIs, Gráficos, Insights]
        E[components/Filtros, Layout]
    end
    subgraph Data Layer
        F[Dados Brutos (CSV, API)]
        G[Dados Consolidados (Parquet)]
        H[cliente_pipeline.py (ETL)]
    end
    F --> H --> G
    G --> D
    D -->|DataFrames| B
    B --> A
```

### Stack Tecnológica

| Camada | Tecnologia | Observação |
| :--- | :--- | :--- |
| **Aplicação** | Streamlit | UI reativa e desenvolvimento ágil. |
| **Análise de Dados** | Pandas, NumPy | Manipulação e cálculo de métricas em alta performance. |
| **Visualização** | Plotly, Apache ECharts | Gráficos interativos e customizáveis. |
| **Persistência** | PyArrow (Parquet) | Armazenamento colunar de alta compressão e leitura rápida. |
| **ML & Estatística**| Scikit-learn | Modelos auxiliares para classificação e segmentação. |
| **Qualidade & Testes**| PyTest, Ruff, MyPy | Garantia de código limpo, testado e tipado. |

---

## 5. Roadmap do Projeto

O InsightX está em constante evolução. Os próximos passos estratégicos incluem:

- [x] Migração completa para Python 3.11 e Streamlit 1.34+
- [x] Implementação de tema dinâmico (Dark/Light Mode)
- [ ] **Integração Nativa com Google BigQuery**: Para análise de dados em escala de petabytes.
- [ ] **Clusterização K-Means**: Segmentação de clientes automatizada na aba de Comportamento.
- [ ] **Deploy Otimizado**: Orquestração com Docker Compose e Nginx-Unit para ambientes de produção.
- [ ] **Modelo de LTV Preditivo**: Projeção do valor do tempo de vida do cliente.

---

## 6. Vamos Conversar?

Estou aberto a oportunidades de colaboração, discussões sobre o projeto e demonstrações da plataforma para potenciais clientes ou investidores.

*   **LinkedIn**: [/brunomendesdeveloper](https://linkedin.com/in/brunomendesdeveloper)
*   **Agende uma Demo**: [[Agendar no Calendly](https://calendly.com/brunomendessj/30min)]
*   **GitHub**: [/mnds-brn001](https://github.com/mnds-brn001)
*   [Saiba Mais](https://insight-expert.carrd.co/)
---

## 7. Licença de Uso

**Copyright (c) 2025 Insight Expert Analytics.**

Este é um projeto de código-fonte fechado (proprietary). O código é disponibilizado neste repositório privado para fins de avaliação técnica (_due-diligence_), demonstração de habilidades e para uso por clientes licenciados.

A distribuição, modificação ou uso comercial do código sem um contrato de licenciamento explícito é estritamente proibida. Para mais informações sobre licenciamento, entre em contato.

<br>
<p align="center"><sub>Feito com ❤️ em Python: transformando dados em ação.</sub></p>
