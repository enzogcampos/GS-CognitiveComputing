

## Cognitive Computing, Computer Vision and IoT Systems | FIAP

Predição de Sucesso em Missões Espaciais com Machine Learning

Tipo de solução: Ciência de Dados / Machine Learning



---

# 1. Problema

A indústria espacial depende de lançamentos bem-sucedidos para garantir o funcionamento de satélites, missões científicas, telecomunicações e serviços de observação da Terra.

Falhas em missões espaciais podem gerar prejuízos financeiros elevados, perda de equipamentos e atrasos em operações estratégicas. Dessa forma, torna-se importante compreender os fatores que influenciam o sucesso ou fracasso de lançamentos espaciais.

---

# 2. Objetivo

Desenvolver um modelo de Machine Learning capaz de prever o sucesso de missões espaciais utilizando dados históricos de lançamentos.

A solução busca identificar padrões associados ao sucesso das missões e demonstrar como técnicas de Ciência de Dados podem apoiar a tomada de decisão no contexto da Economia Espacial.

---

# 3. Dados Utilizados

Foi utilizada uma base pública contendo informações históricas de missões espaciais realizadas por diferentes empresas e organizações ao redor do mundo.

### Arquivo utilizado

**Space_Corrected.csv**


---

# 4. Fonte dos Dados

Dataset público disponibilizado pela comunidade Kaggle:

https://www.kaggle.com/datasets/agirlcoding/all-space-missions-from-1957/data

Ferramentas utilizadas:

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

---

# 5. Tratamento


Foram realizadas análises iniciais utilizando:

* df.head()
* df.info()
* df.describe()
* df.isnull().sum()

* Remoção de espaços nos nomes das colunas;
* Tratamento dos valores ausentes da coluna Rocket;
* Criação da variável alvo Sucesso.

A variável alvo foi definida como:

* Success = 1
* Failure = 0
* Partial Failure = 0
* Prelaunch Failure = 0


Divisão dos dados:

* Treino: 70%
* Teste: 30%

---

# 6. Análises Realizadas

A análise exploratória mostrou que a maior parte dos lançamentos espaciais
registrados foi realizada por grandes organizações governamentais e empresas
do setor aeroespacial.

Também foi possível identificar os países com maior número de lançamentos,
destacando Rússia, Eua e Cazaquistão como os principais participantes da
atividade espacial histórica.

Após o treinamento do modelo Random Forest, a matriz de confusão
demonstrou que o modelo identificou corretamente 1.152 missões bem
sucedidas, apresentando ótimo desempenho para previsão de sucessos.

A base de dados é desbalanceada, contendo aproximadamente 90% de
missões bem sucedidas e apenas 10% de falhas, o que impactou a capacidade
do modelo em identificar missões fracassadas.

---




