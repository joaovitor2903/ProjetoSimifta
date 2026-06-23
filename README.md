# Projeto SIMIFTA: Previsão de Visitantes nos POIs de São Miguel

**Grupo 2**
* João Costa (113564)
* Sílvia Ribeiro (129428)
* Vitória Rodrigues (130557)

## Objetivo do Projeto
O objetivo deste projeto é prever o volume de afluência (total_incoming) em quatro pontos de interesse (POIs) da ilha de São Miguel, Açores, com 24 horas de antecedência.

O modelo visa apoiar a gestão do turismo sustentável através do cálculo de um "Crowding Factor". Se a taxa de ocupação prevista ultrapassar 80% da capacidade histórica, o sistema dispara um alerta de risco de sobrelotação (Alerta GSTC A8), permitindo ações preventivas.

## Instruções de Reprodução

### 1. Estrutura de Pastas
Para que o código funcione corretamente, a raiz do projeto deve conter a seguinte estrutura:

PROJETO_RAIZ/

├── dataset/   # Pasta com todos os ficheiros .csv

├── notebooks/                # Ficheiros .ipynb

├── README.md

└── requirements.txt

### 2. Dependências
Para garantir a reprodutibilidade e evitar conflitos entre bibliotecas, recomendamos vivamente a criação de um ambiente virtual dedicado ao projeto:

**No Windows:**
```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```
**No macOS ou Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### 3. Ordem de Execução
Para reproduzir os resultados, os notebooks devem ser executados pela seguinte ordem sequencial:

01_integracaoDados.ipynb

02_PreProcessamento.ipynb

03_AnaliseExploratoria.ipynb

04_DecomposicaoSerieTemporal.ipynb

05_Modelacao_Preditiva_e_Contexto.ipynb

06_Modelacao_Preditiva_e_Contexto_segundo.ipynb

Os notebooks detetarão automaticamente a pasta dataset e exportarão os resultados para a subpasta dataset/export_model/.
