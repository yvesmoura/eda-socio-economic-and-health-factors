# <p align="center"> Aprendizagem não supervisionada com base em dados nacionais </p> 
<p align="center"><img src="https://github.com/yvesmoura/eda-socio-economic-and-health-factors/blob/eda-yves/img/desafio_final.jpg?raw=true"></p>


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

<p align="center"><img src="https://github.com/yvesmoura/eda-socio-economic-and-health-factors/blob/eda-yves/img/hp-1.png?raw=true"></p>

  **Verdade**, paises que tem maiores investimento na saude tendem a ter uma expectativa de vida mais alta.

- **2. Países com maior número de filhos por mulher (total_fer) tendem a ter uma expectativa de morte de criança mais alta(child_mort).** 

<p align="center"><img src="https://github.com/yvesmoura/eda-socio-economic-and-health-factors/blob/eda-yves/img/hp-2.png?raw=true"></p>

  **Verdade**, Quanto maior a quantidade de filhos pela mulher tentem a ter uma expectativa de morte de criança maior.

- **3. Países com maior lucro líquido por pessoa(income) tendem a ter uma expectativa de pib per capita mais alta(gdpp).** 

<p align="center"><img src="https://github.com/yvesmoura/eda-socio-economic-and-health-factors/blob/eda-yves/img/hp-3.png?raw=true"></p>

  **Verdade**, Países com maior lucro líquido por pessoa tendem a ter uma expectativa de pib per capita mais alta.

- **4. Países com exportações de bens(exports) tendem a ter uma menor importações de bens(imports).** 

<p align="center"><img src="https://github.com/yvesmoura/eda-socio-economic-and-health-factors/blob/eda-yves/img/hp-4.png?raw=true"></p>

  **Falso**, Quanto maior a exportações tendem a ter maior importacoes de bens.

- **5. Países com maiores gastos totais com saúde per capita (health) tendem a ter uma expectativa menor de morte de criança menores de 5 anos(child_mort).** 

<p align="center"><img src="https://github.com/yvesmoura/eda-socio-economic-and-health-factors/blob/eda-yves/img/hp-5.png?raw=true"></p>

  **Falso**, países que investem consideravelmente em saúde muitas vezes estejam no mesmo patamar de desenvolvimento que países que investem menos.


## Análise Multivariada

### Essas análises nos revelam algumas coisas: 

- Podemos isolar os países com menores desempenho em atributos-chave já destacados acima (mortalidade infantil, expectativa de vida e inflação);

- Podemos ver se há países com baixo desenvolvimento em mais de um desses atributos-chave(o que faria deles melhores candidatos para receberem os benefócios);
    
- Podemos ver se há países com baixo desenvolvimento em um atributo, mas com alto em outro ( nesse caso, seria um país com menor chance de ser escolhido para o benefício);



### Assim, podemos concluir que:

 - Até então, os melhores candidatos para receber os benefícios são:
    - Podemos isolar os países com menores desempenho em atributos-chave já destacados acima (mortalidade infantil, expectativa de vida e inflação);

        1) Republica central africana (Alta taxa de mortalidade intanfil e e baixa expectativa de vida);

        2) Haiti (Alta taxa de mortalidade intanfil e e baixa expectativa de vida);

        3) Serra Leoa(taxa de mortalidade infantil alta);

        4) Chad (taxa de mortalidade infantil alta)

        5) Lesotho (baixa expectativa de vida)

        6) Guiné equatorial (alta inflação)

        7) timor-leste (alta inflação)

        8) Mongolia (alta inflação)

        9) Nigéria (alta inflação)

        10) Níger (alta taxa de filhos por mulher)

Nenhum deles aparece como um país destaque em outro atributo
        

------------------------------------------------------------


## Próximas etapas/melhorias

- Aprimorar a análise de bivariância, explorando relações entre variáveis de forma mais detalhada.

- Testar outros modelos de análise multivariada além do método de Pearson, por exemplo o método Spearman
- Desenvolver um dashboard para gestão, utilizando ferramentas como Power BI ou Streamlit, para oferecer uma visualização mais dinâmica e interativa dos dados e insights obtidos.


## Autores

- [@IgorPinheiro09](https://www.github.com/IgorPinheiro09)
- [@Nandobrcmiranda](https://www.github.com/Nandobrcmiranda)
- [@PedreiraVictor](https://www.github.com/PedreiraVictor)
- [@yvesmoura](https://www.github.com/yvesmoura)