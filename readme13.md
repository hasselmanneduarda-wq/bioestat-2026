# Tarefa 13: Aplicação de Distribuições de Probabilidade em Ciências Biológicas

## 👥 Integrantes

* André Luiz Leal
* Maria Eduarda Hasselman
* Raissa Lara Pinheiro

## 📊 Base de Dados

* **Nome:** Iris Dataset
* **Instituição responsável:** UCI Machine Learning Repository (originado do estudo clássico de Ronald A. Fisher, 1936).
* **Link de acesso à base:** [UCI Machine Learning Repository - Iris](https://archive.ics.uci.edu/ml/datasets/iris)
* **Link direto para os dados raw:** [iris.data (UCI)](https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data)

## 📚 Fontes e Referências

* BUSSAB, W. O.; MORETTIN, P. A. **Estatística básica**. 9. ed. São Paulo: Saraiva, 2017.
* FISHER, R. A. The use of multiple measurements in taxonomic problems. **Annals of Eugenics**, v. 7, n. 2, p. 179–188, 1936.
* SCIPY COMMUNITY. **scipy.stats**. Disponível em: <https://docs.scipy.org/doc/scipy/reference/stats.html>.
* UCI MACHINE LEARNING REPOSITORY. **Iris Dataset**. Disponível em: <https://archive.ics.uci.edu/dataset/53/iris>.

## Instruções de Reprodução da Análise


1. **Acesse a plataforma do Colab:**
   Navegue até o [Google Colab](https://colab.research.google.com/).

2. **Crie um novo Notebook:**
   Clique em `Novo notebook` (`New notebook`).

3. **Instale/Importe os pacotes na primeira célula:**
   ```python
   import matplotlib.pyplot as plt
   import numpy as np
   import pandas as pd
   import scipy.stats as stats
```

4. **Carregue a base de dados na segunda célula:**
   ```python
   url = "https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data"
   cols = [
       "sepal_length",
       "sepal_width",
       "petal_length",
       "petal_width",
       "species",
   ]
   df = pd.read_csv(url, header=None, names=cols)
   df.head()
```

5. **Execute os cálculos e visualizações:**
   Crie células subsequentes para calcular probabilidades (usando `.cdf()`, `.sf()`, `.ppf()`) e plote os gráficos interativamente utilizando `matplotlib.pyplot`.