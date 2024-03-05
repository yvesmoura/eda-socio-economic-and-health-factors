# <p align="center">🏪💊 ROSSMANN STORE SALES PREDICTION 💊🏪</p> 
<p align="center"><img src="https://github.com/yvesmoura/eda-socio-economic-and-health-factors/blob/eda-yves/img/desafio_final.jpg?raw=true"></p>
<br>



## Rodando localmente

Clone o projeto

```bash
  git clone https://github.com/yvesmoura/eda-socio-economic-and-health-factors.git
```

Entre no diretório do projeto

```bash
  cd eda-socio-economic-and-health-factors
```

Criar ambiente de desenvolvimento

```bash
  * python3 -m venv eda

  * source eda/bin/activate
```


Instale as dependências

```bash
  pip install -r rquirements.txt
```

<br>

 ### - Importing Dataset:

* Kaggle: https://www.kaggle.com/datasets/rohan0301/unsupervised-learning-on-country-data

<br>

 ### - Data Dictionary

O Dataset usado para este projeto possui 167 linhas e 10 colunas. Os dados contém:


| Variable                       | Descriptions                                                 |
| -------------------------------| ------------------------------------------------------------ |
| country                        | Nome do país|
| child_mort                     | Morte de crianças menores de 5 anos por 1.000 nascidos vivos |
| exports                        | Exportações de bens e serviços per capita. Dado como %idade do PIB per capita                               |
| health                         |     Gastos totais com saúde per capita. Dado como %idade do PIB per capita                  |
| imports                        | Importações de bens e serviços per capita. Dado como %idade do PIB per capita |
| income                         | Lucro líquido por pessoa|
| inflation                      | A medição da taxa de crescimento anual do PIB total |
| life_expec                     |  O número médio de anos que uma criança recém-nascida viveria se os atuais padrões de mortalidade  |
| total_fer                      | O número de filhos que nasceriam de cada mulher se as atuais taxas de fertilidade por idade permanecessem as mesmas. |
| gdpp                      | O PIB per capita. Calculado como o PIB total dividido pela população total. |