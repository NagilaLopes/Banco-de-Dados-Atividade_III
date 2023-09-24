# Resolução Atividade III - SQL

<h2>1º Questão</h2>
Selecione todos os dados dos países da tabela_paises.
 
    ```select * from tabela_paises;```

<h2>Resultado esperado</h2>

![questão 1](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/eacc6d9a-8ae9-4e2e-a82b-1c79f10e2c7c)


<h2>2º Questão</h2>
Selecione todas as cidades cujo país seja brazil.

```select cidade from tabela_paises where pais ='Brazil';```

<<h2>Resultado esperado</h2>

![questão 2](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/dec246b4-d2d5-46d7-83a0-b0fe7f27a9fa)


<h2>3º Questão</h2>
Selecione todas as cidades cuja região(estado) é ceará.

```select cidade from tabela_paises where regiao = 'Ceará';```

<h2>Resultado esperado</h2>

![questão 3](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/5d137782-2e3a-49ca-98fa-5605a1d012d8)


<h2>4º Questão</h2>
Utilize a função count para saber quantas regiões(estados) existem na China,
utilize também o group by;

```select count(regiao) from tabela_paises where pais = 'China' group by pais;```

<h2>Resultado esperado</h2>

![questão 4](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/8d0e146b-7ed7-44f1-bf0a-ad0d30435acf)


<h2>5º Questão</h2>
 Quais regiões, diferentes, existem no Canadá?

 ```select distinct regiao from tabela_paises where pais = 'Canada';```

<h2>Resultado esperado</h2>

![questão 5](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/6f949cf9-15af-45bd-9ae7-c8270469b260)


<h2>6º Questão</h2>
Quantos países diferentes existem na tabela 'tabela_paises'.

```select count(distinct pais) from tabela_paises;```

<h2>Resultado esperado</h2>

![questão 6](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/8f0c96a1-7500-4c5a-847f-3ebbd9b0e105)


<h2>7º Questão</h2>
Quantas cidades diferentes existem no brazil.

```select count(distinct regiao) from tabela_paises where pais ='Brazil';```

<h2>Resultado esperado</h2>

![questão 7](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/ab16092b-8a20-438e-986e-30aa3cbb2cd9)


<h2>8º Questão</h2>
 Selecione os países e quantas regiões cada país possui.

 ```select pais, count(distinct regiao) as regioes from tabela_paises group by pais;```
 
<h2>Resultado esperado</h2>

![questão 8](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/5ea847cb-1ba8-4aaf-9cf6-17369cdc8872)


<h2>9º Questão</h2>
Quantas pessoas com nome começando em 'João' existem no banco?

```select count(*) from tabela_paises where nome ='Joao';```

<h2>Resultado esperado</h2>

![questão 9](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/8c147286-2ab9-48c7-8caf-4560dd35c98f)


<h2>10º Questão</h2>
Quantas pessoas têm o nome John?

```select count(*) from tabela_paises where nome ='John';```

<h2>Resultado esperado</h2>

![questão 9](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/0fb03c2f-f769-4e18-918a-d207d615be41)


<h2>11 Questão</h2>
Ordene os nomes dos países sem repetição em ordem alfabética.

```select distinct pais from tabela_paises order by pais```

<h2>Resultado esperado</h2>


![questão 11](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/2f8733d8-df5a-4a38-bfe9-ae209079852e)
