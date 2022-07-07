# Projeto_house_sale
Projeto de regressão linear utilizando o dataset 'House Sales in King County, USA'

# Contextualização

O dataset utilizado contêm informações relativas ao preço das casas vendidas entre maio 2014 e maio de 2015 em King County. Este dataset foi obtido no Kaggle.

A ideia do projeto é estimar uma modelo de regressão linear que seja capaz de estimar o preço do imóvel dado um conjunto de características, entanto, para que isso seja possível antes será necessária realizar algumas fases para alcançar o objetivo.

A primeira parte é a de análise exploratória dos dados, onde foi observado os dados presentes no dataset, além do comportamento e distribuição de frequência da variável dependente (Price).

Depois disso, os dados foram transformados como forma de tratar a assimetria encontrada, visto que para atingir o objetivo precisamos que os dados se comportem como uma distribuição normal. Além disso, foram observadas algumas estatísticas estimadas pelo modelo de minimos quadrados ordinários(OLS), com a finalidade identificar os valores de R² e R² ajustado, o teste F e os testes T.

Por fim utilizaremos o Scikit Learn para criar um modelo de regressão linear (LinearRegression) que nos permita prever o valor do imóvel com base nas características selecionadas.

O desenvolvimento do projeto pode ser visto no Notebook [Modelo_regressaolinear](https://github.com/MateusSampaio1/Projeto_house_sale/blob/main/Notebook/Modelo_regressaolinear.ipynb)

# Fonte
**Kaggle**: https://www.kaggle.com/datasets/harlfoxem/housesalesprediction?resource=download

# Dicionário dos dados
- **id** - Id da casa à venda;
- **date** - Data de venda da casa;
- **price** - Preço que a casa foi vendida (USD);
- **bedrooms** - Número de quartos;
- **bathrooms** - Número de banhaeiros(Foi considerado como 0.5 um quarto que possui banheiro sem chuveiro);
- **sqft_living** - Espaço interior do imóvel (Em pés quadrados);
- **sqft_lot** - Tamanho de todo o terreno (Em pés quadrados);
- **floors** - Qtd de andares;
- **waterfront** - Variável binária que indica se o imóvel é ou não na orla da praia;
- **view** - Corresponde a um índice que varia de 0 a 4 e tenta traduzir quão boa é a vista do imóvel;
- **condition** - Corresponde a um índice que vai de 1 a 5 e é referente a condição do imóvel;
- **grade** - Um índice que vai de 1 a 13 e diz respeito ao nível de construção e design do imóvel;
- **sqft_above** - Indica o espaço interno do imóvel que se encontra acima do nível do solo (Em pés quadrados);
- **sqft_basement** - Indica o espaço interno do imóvel que se encontra abaixo do nível do solo (Em pés quadrados);
- **yr_built** - Ano de construção da casa;
- **yr_renovated** - Ano da última reforma realizada no imóvel;
- **zipcode**  - CEP do imóvel;
- **lat** - Latitude;
- **long** - Longitude;
- **sqft_living15** - O espaço interior dos imóveis dos 15 vizinhos mais próximos (Em pés quadrados)
- **sqft_lot15** - O tamanho médio dos terrenos dos 15 vizinhos mais próximos (Em pés quadrados)
