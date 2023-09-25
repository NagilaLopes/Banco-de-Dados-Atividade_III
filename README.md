# Resolução Atividade III - SQL

<h2>1º Questão</h2>
Selecione todos os dados dos países da tabela_paises.

   ```select * from tabela_paises;```

<h2>Resultado esperado</h2>

![questão 1](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/199477e3-8efb-4cd0-95c4-48fa8a65d128)


<h2>2º Questão</h2>
Selecione todas as cidades cujo país seja brazil.

```select cidade from tabela_paises where pais ='Brazil';```

<h2>Resultado esperado</h2>

![questão 2](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/117e37eb-3609-4a9b-a6a6-7b83a4a01d47)


<h2>3º Questão</h2>
Selecione todas as cidades cuja região(estado) é ceará.

```select cidade from tabela_paises where regiao = 'Ceará';```

<h2>Resultado esperado</h2>

![questão 3](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/e3222a11-c497-4fe6-821b-c6a8042a336d)


<h2>4º Questão</h2>
Utilize a função count para saber quantas regiões(estados) existem na China,
utilize também o group by;

```select count(regiao) from tabela_paises where pais = 'China' group by pais;```

<h2>Resultado esperado</h2>

![questão 4](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/d1d1a774-3192-4fa6-876d-be445b99f5c8)


<h2>5º Questão</h2>
 Quais regiões, diferentes, existem no Canadá?

 ```select distinct regiao from tabela_paises where pais = 'Canada';```

<h2>Resultado esperado</h2>

![questão 5](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/74d4c724-b008-4cbf-87ed-677fdf0edec0)


<h2>6º Questão</h2>
Quantos países diferentes existem na tabela 'tabela_paises'.

```select count(distinct pais) from tabela_paises;```

<h2>Resultado esperado</h2>

![questão 6](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/2c0d2390-19cb-4ae1-96f8-ae6526654355)


<h2>7º Questão</h2>
Quantas cidades diferentes existem no brazil.

```select count(distinct regiao) from tabela_paises where pais ='Brazil';```

<h2>Resultado esperado</h2>

![questão 7](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/46e23f09-7981-43e9-a99a-d29ea730cb19)


<h2>8º Questão</h2>
 Selecione os países e quantas regiões cada país possui.

 ```select pais, count(distinct regiao) as regioes from tabela_paises group by pais;```
 
<h2>Resultado esperado</h2>

![questão 8](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/560c48f3-b0df-4c09-ae24-0d6f25839257)


<h2>9º Questão</h2>
Quantas pessoas com nome começando em 'João' existem no banco?

```select count(*) from tabela_paises where nome ='Joao';```

<h2>Resultado esperado</h2>

![questão 9](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/8fe6649f-be17-49d0-b58d-216c37ed3521)


<h2>10º Questão</h2>
Quantas pessoas têm o nome John?

```select count(*) from tabela_paises where nome ='John';```

<h2>Resultado esperado</h2>

![questão 10](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/bd20b549-ec80-4acd-b4b5-69b2af595584)


<h2>11 Questão</h2>
Ordene os nomes dos países sem repetição em ordem alfabética.

```select distinct pais from tabela_paises order by pais```

<h2>Resultado esperado</h2>

![questão 11](https://github.com/NagilaLopes/Banco-de-Dados-Atividade_III/assets/111643449/501cd686-bd07-4d28-872e-afb2fae31215)

