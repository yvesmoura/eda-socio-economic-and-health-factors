# <p align="center"> Aprendizagem não supervisionada com base em dados nacionais </p> 
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

## - Importando conjunto de dados:

* Kaggle: https://www.kaggle.com/datasets/rohan0301/unsupervised-learning-on-country-data

<br>

## - Dicionário de dados

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



## - Hipótese principal escolhida


- **1. Países com maiores gastos totais com saúde per capita (health) tendem a ter uma expectativa de vida mais alta (life_expec).** 

- **2. Países com maior número de filhos por mulher (total_fer) tendem a ter uma expectativa de morte de criança mais alta(child_mort).** 

- **3. Países com maior lucro líquido por pessoa(income) tendem a ter uma expectativa de pib per capita mais alta(gdpp).** 

- **4. Países com exportações de bens(exports) tendem a ter uma menor importações de bens(imports).** 

- **5. Países com maiores gastos totais com saúde per capita (health) tendem a ter uma expectativa menor de morte de criança menores de 5 anos(child_mort).** 


## Próximas etapas/melhorias


## Autores

- [@IgorPinheiro09](https://www.github.com/IgorPinheiro09)
- [@Nandobrcmiranda](https://www.github.com/Nandobrcmiranda)
- [@PedreiraVictor](https://www.github.com/PedreiraVictor)
- [@yvesmoura](https://www.github.com/yvesmoura)