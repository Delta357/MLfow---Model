# MLflow machine learnig 

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
[![author](https://img.shields.io/badge/author-RafaelGallo-red.svg)](https://github.com/RafaelGallo?tab=repositories) 
[![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-374/) 
[![](https://img.shields.io/badge/R-3.6.0-red.svg)](https://www.r-project.org/)
[![](https://img.shields.io/badge/ggplot2-white.svg)](https://ggplot2.tidyverse.org/)
[![](https://img.shields.io/badge/dplyr-blue.svg)](https://dplyr.tidyverse.org/)
[![](https://img.shields.io/badge/readr-green.svg)](https://readr.tidyverse.org/)
[![](https://img.shields.io/badge/ggvis-black.svg)](https://ggvis.tidyverse.org/)
[![](https://img.shields.io/badge/Shiny-red.svg)](https://shiny.tidyverse.org/)
[![](https://img.shields.io/badge/plotly-green.svg)](https://plotly.com/)
[![](https://img.shields.io/badge/XGBoost-red.svg)](https://xgboost.readthedocs.io/en/stable/#)
[![](https://img.shields.io/badge/Tensorflow-orange.svg)](https://powerbi.microsoft.com/pt-br/)
[![](https://img.shields.io/badge/Keras-red.svg)](https://powerbi.microsoft.com/pt-br/)
[![](https://img.shields.io/badge/CUDA-gree.svg)](https://powerbi.microsoft.com/pt-br/)
[![](https://img.shields.io/badge/Caret-orange.svg)](https://caret.tidyverse.org/)
[![](https://img.shields.io/badge/Pandas-blue.svg)](https://pandas.pydata.org/) 
[![](https://img.shields.io/badge/Matplotlib-blue.svg)](https://matplotlib.org/)
[![](https://img.shields.io/badge/Seaborn-green.svg)](https://seaborn.pydata.org/)
[![](https://img.shields.io/badge/Matplotlib-orange.svg)](https://scikit-learn.org/stable/) 
[![](https://img.shields.io/badge/Scikit_Learn-green.svg)](https://scikit-learn.org/stable/)
[![](https://img.shields.io/badge/Numpy-white.svg)](https://numpy.org/)
[![](https://img.shields.io/badge/PowerBI-red.svg)](https://powerbi.microsoft.com/pt-br/)

![Logo](https://devclass.com/wp-content/uploads/2018/10/MLflow-logo.png)


## Projeto

- Modelo produção com MLFlow ciclo modelo machine learning.


## Stack utilizada

**Programação** Python

**Leitura CSV**: Pandas

**Análise de dados**: Seaborn, Matplotlib

**Machine learning**: Scikit-learn

**Ciclo de vida do modelo machine learning**: MLflow




## Variáveis de Ambiente

Para rodar esse projeto, você vai precisar adicionar as seguintes variáveis de ambiente no seu .env

Instalando a virtualenv

`pip install virtualenv`

Nova virtualenv

`virtualenv nome_virtualenv`

Ativando a virtualenv

`source nome_virtualenv/bin/activate` (Linux ou macOS)

`nome_virtualenv/Scripts/Activate` (Windows)

Retorno da env

`projeto_py source venv/bin/activate` 

Desativando a virtualenv

`(venv) deactivate` 

Instalando pacotes

`(venv) projeto_py pip install flask`

Instalando as bibliotecas

`pip freeze`


# Ciclo modelo machine learning

![Logo](https://lh4.googleusercontent.com/rwaMzrCLImiQtWVp0g5lcKS_Q82xaizNjHq2B3B0Cj93UL1kMREDOMsVJ-9yExH498z_elQPmiE43yILSxpl-HMmuvbTgacDMUmw4kIsOvowJKqCXHlEQSqEDeGWZsAMM78CJTv4)


## Instalação

Instalação das bibliotecas para esse projeto no python.

```bash
  conda install -c conda-forge pandas 
  conda install -c conda-forge scikitlearn
  conda install -c conda-forge numpy
  conda install -c conda-forge scipy
  conda install -c conda-forge mlflow 

  python==3.6.4
  numpy==1.13.3
  scipy==1.0.0
  matplotlib==2.1.2
  mlflow==1.22.0
```
Instalação do Python É altamente recomendável usar o anaconda para instalar o python. Clique aqui para ir para a página de download do Anaconda https://www.anaconda.com/download. Certifique-se de baixar a versão Python 3.6. Se você estiver em uma máquina Windows: Abra o executável após a conclusão do download e siga as instruções. 

Assim que a instalação for concluída, abra o prompt do Anaconda no menu iniciar. Isso abrirá um terminal com o python ativado. Se você estiver em uma máquina Linux: Abra um terminal e navegue até o diretório onde o Anaconda foi baixado. 
Altere a permissão para o arquivo baixado para que ele possa ser executado. Portanto, se o nome do arquivo baixado for Anaconda3-5.1.0-Linux-x86_64.sh, use o seguinte comando: chmod a x Anaconda3-5.1.0-Linux-x86_64.sh.

Agora execute o script de instalação usando.


Depois de instalar o python, crie um novo ambiente python com todos os requisitos usando o seguinte comando

```bash
conda env create -f environment.yml
```
Após a configuração do novo ambiente, ative-o usando (windows)
```bash
activate "Nome do projeto"
```
ou se você estiver em uma máquina Linux
```bash
source "Nome do projeto" 
```
Agora que temos nosso ambiente Python todo configurado, podemos começar a trabalhar nas atribuições. Para fazer isso, navegue até o diretório onde as atribuições foram instaladas e inicie o notebook jupyter a partir do terminal usando o comando
```bash
jupyter notebook
```
    
## Demo rede neural 

```bash
  # Carregando as bibliotecas 
  import pandas as pd
  import seaborn as sns
  import matplotlib.pyplot as plt

  # Carregando o dataset
  data = pd.read_csv("data.csv")
  
  # Visualizando os 5 primeiros itens
  data.head()

  # visualizando linhas e colunas com shape
  data.shape

  # Informações das variaveis
  data.info()

  # Definindo variaveis para modelo
  x = dados.iloc[:, 0:8].values
  y = dados.iloc[:, 1].values

  # Treinamento do modelo
  from sklearn.model_selection import train_test_split
  X_train, x_test, y_train, y_test = train_test_split(X, y, test_size = 0.2)

  # Mlflow
  import mlflow
  mlflow.set_experiment('nome_do_projeto')

  # Modelo regressão linear
  from sklearn.linear_model import LinearRegression
  lr = LinearRegression()
  lr.fit(X_train, y_train)
  lr_predicted = lr.predict(X_test)

  # modelo mlflow
  mlflow.sklearn.log_model(lr, "lr")

  # Métricas
  import math
  from sklearn.metrics import mean_absolute_error
  from sklearn.metrics import mean_squared_error
  from sklearn.metrics import r2_score

  mse = mean_squared_error(y_test, lr_predicted)
  rmse =  math.sqrt(mse)
  r2 = r2_score(y_test, lr_predicted)

  # Rodando o mlflow
  mlflow.get_experiment_by_name('nome_do_projeto')

  # API
  mlflow.list_run_infos('1')

  # Rodando a aplicação
  mlflow.get_run('7e88da39569343e3ac29cba3710938c8')

```


## Melhorias

Que melhorias você fez no seu código? 
- Ex: refatorações, melhorias de performance, acessibilidade, etc


## Suporte

Para suporte, mande um email para rafaelhenriquegallo@gmail.com

