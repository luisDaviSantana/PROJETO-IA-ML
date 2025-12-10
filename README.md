# Projeto: Fundamentos Práticos de IA/ML

Análise exploratória do dataset Titanic e implementação de modelos básicos de ML.

# Fundamentos Práticos de IA/ML

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.1%2B-orange)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.3%2B-red)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![GitHub](https://img.shields.io/badge/GitHub-Repository-black)
![License](https://img.shields.io/badge/License-MIT-green)

**Última Atualização:** $(date +%d/%m/%Y)

## 📋 Sobre o Projeto

Este projeto implementa os fundamentos práticos de Data Science e Machine Learning através de dois estudos de caso completos:

1. **📊 Análise Exploratória do Titanic** - Estatística descritiva com pandas
2. **🤖 Classificação com Dataset Iris** - Pipeline completo de ML com scikit-learn

## 🎯 Objetivos Alcançados

### ✅ **PARTE 1: Estatística Básica na Prática**
- **Dataset:** Titanic (Kaggle)
- **Análise:** Média, mediana, desvio padrão, correlações, distribuições
- **Técnicas:** Identificação e tratamento de valores faltantes
- **Resultado:** `"Analisei dados com pandas, identifiquei correlações entre variáveis e lidei com valores faltantes"`

### ✅ **PARTE 2: ML Básico com scikit-learn**
- **Dataset:** Iris (scikit-learn)
- **Modelos Implementados:**
  - Regressão Logística (classificação)
  - Árvore de Decisão (classificação)
  - K-Means (clustering não supervisionado)
- **Pipeline Completo:** Pré-processamento → Treino → Avaliação → Validação Cruzada
- **Resultado:** `"Implementei um classificador para dataset Iris com 98% de acurácia, usando validação cruzada"`

### ✅ **PARTE 3: Ambiente Profissional**
- **VS Code + Jupyter Notebook** configurado
- **Git & GitHub** com versionamento
- **Estrutura de Projeto** organizada

## 📊 Resultados Destacados

### Titanic Analysis
| Métrica | Valor | Insight |
|---------|-------|---------|
| **Correlação Pclass-Survived** | -0.34 | Passageiros de classe mais alta sobreviveram mais |
| **Sobrevivência por Sexo** | 74% mulheres vs 19% homens | "Women and children first" comprovado |
| **Valores Faltantes Tratados** | Age (20%), Cabin (77%) | Estratégias específicas por coluna |
| **Taxa Sobrevivência Geral** | 38.4% | Baseline para modelos |

### Iris Classification
| Modelo | Acurácia Teste | Validação Cruzada | Observação |
|--------|----------------|-------------------|------------|
| **Regressão Logística** | 98% | 96% (±4%) | Com feature scaling |
| **Árvore de Decisão** | 98% | 95% | max_depth=3, feature importance |
| **K-Means** | Silhouette: 0.55 | 3 clusters | Identificou espécies naturais |

## 🗂️ Estrutura do Projeto
projeto-ia-ml/
├── 📁 notebooks/ # Jupyter Notebooks completos
│ ├── 1_analise_exploratoria_titanic.ipynb
│ └── 2_ml_basico_sklearn.ipynb
├── 📁 data/ # Estrutura de dados
│ ├── raw/ # Dados brutos (local)
│ └── processed/ # Dados processados (local)
├── 📁 src/ # Código fonte modular
├── 📁 models/ # Modelos treinados (local)
├── 📄 requirements.txt # Dependências do projeto
├── 📄 .gitignore # Arquivos ignorados no Git
├── 📄 README.md # Esta documentação
└── 📄 config.py # Configurações do projeto


## 🛠️ Tecnologias Utilizadas

| Tecnologia | Versão | Uso no Projeto |
|------------|--------|----------------|
| **Python** | 3.9+ | Linguagem principal |
| **Pandas** | 2.1+ | Manipulação e análise de dados |
| **NumPy** | 1.24+ | Computação numérica |
| **Matplotlib** | 3.8+ | Visualizações básicas |
| **Seaborn** | 0.13+ | Visualizações estatísticas |
| **Scikit-learn** | 1.3+ | Machine Learning |
| **Jupyter** | 7.0+ | Notebooks interativos |
| **Git** | - | Controle de versão |

## 🚀 Como Executar

### Pré-requisitos
- Python 3.9 ou superior
- Git instalado

### Passo a Passo

```bash
# 1. Clone o repositório
git clone https://github.com/SEU-USUARIO/PROJETO-IA-ML.git
cd fundamentos-ia-ml

# 2. Crie e ative ambiente virtual
python -m venv venv
# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate

# 3. Instale dependências
pip install -r requirements.txt

# 4. Baixe os dados
# Opção A: Manualmente
# - Acesse: https://www.kaggle.com/c/titanic/data
# - Baixe train.csv e coloque em data/raw/

# Opção B: Via script (crie download_data.py)
# python scripts/download_data.py

# 5. Execute os notebooks
jupyter notebook notebooks/
