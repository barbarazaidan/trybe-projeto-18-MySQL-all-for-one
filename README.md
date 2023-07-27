# Projeto MYSQL All For One
## Este repositório contém o desenvolvimento do meu 18º projeto na Trybe

Seguindo no Backend, chegou o momento de ter o primeiro contato como o banco de dados MySQL. Neste projeto, o objetivo foi trabalhar com o uso de tabelas, fixando vários conceitos relacionados a BD. Para isso, recebi tabelas não normalizadas que precisaram ser normalizadas e populadas. Em seguida, tive que executar diferentes queries para encontrar as informações pedidas ao longo dos requisitos. 

## Detalhes do projeto

Confira os requisitos exigidos pela Trybe (texto extraído dos readme oficial da Trybe):

**1. Normalize as tabelas da planilha SpotifyClone e depois crie as tabelas no banco de dados**

<details><summary>Detalhes</summary>
<p>

Seu banco de dados deve seguir as regras de negócio e ser capaz de recuperar:

> Informações sobre quais planos estão disponíveis e seus detalhes.
* Cada pessoa usuária pode possuir apenas um plano.

> Informações sobre todas as pessoas artistas.
* Uma pessoa artista pode ter vários álbuns;
* Uma pessoa artista pode ser seguida por várias pessoas usuárias.

> Informações sobre todos os álbuns de cada artista.
* Para fins deste projeto, considere que cada álbum possui apenas uma pessoa artista como principal;
* Cada álbum possui várias canções.

> Informações sobre todas as canções de cada álbum.
* Para fins deste projeto, considere que cada canção está contida em apenas um álbum.

> Informações sobre todas as pessoas usuárias, seus planos, seu histórico de reprodução e pessoas artistas seguidas.
* Uma pessoa usuária pode possuir apenas um plano;
* Cada música do histórico de reprodução pode aparecer uma única vez por pessoa (para simplificar, considere que o objetivo do histórico é saber quais canções já foram reproduzidas e não quantas vezes foram reproduzidas);
* Uma pessoa usuária pode seguir várias pessoas artistas, mas cada pessoa artista pode ser seguida apenas uma vez por pessoa usuária.

</p>
</details>

**2. Crie uma QUERY que exiba três colunas:**

<details><summary>Detalhes</summary>
<p>

> A primeira coluna deve exibir a quantidade total de canções. Dê a essa coluna o alias "cancoes".

> A segunda coluna deve exibir a quantidade total de artistas e deverá ter o alias "artistas".

> A terceira coluna deve exibir a quantidade de álbuns e deverá ter o alias "albuns".

</p>
</details>

**3. Crie uma QUERY que deverá ter apenas três colunas:**
<details><summary>Detalhes</summary>
<p>

> A primeira coluna deve possuir o alias "pessoa_usuaria" e exibir o nome da pessoa usuária.

> A segunda coluna deve possuir o alias "musicas_ouvidas" e exibir a quantidade de músicas ouvida pela pessoa com base no seu histórico de reprodução.

> A terceira coluna deve possuir o alias "total_minutos" e exibir a soma dos minutos ouvidos pela pessoa usuária com base no seu histórico de reprodução.

> Os resultados devem estar agrupados pelo nome da pessoa usuária e ordenados em ordem alfabética.

</p>
</details>

**4. Crie uma QUERY que deve mostrar as pessoas usuárias que estavam ativas a partir do ano de 2021, se baseando na data mais recente no histórico de reprodução**

<details><summary>Detalhes</summary>
<p>

> A primeira coluna deve possuir o alias "pessoa_usuaria" e exibir o nome da pessoa usuária.

> A segunda coluna deve ter o alias "status_pessoa_usuaria" e exibir se a pessoa usuária está ativa ou inativa.

> O resultado deve estar ordenado em ordem alfabética.

</p>
</details>

**5. Estamos fazendo um estudo das músicas mais tocadas e precisamos saber quais são as duas músicas mais tocadas no momento. Crie uma QUERY que possua duas colunas:**

<details><summary>Detalhes</summary>
<p>

> A primeira coluna deve possuir o alias "cancao" e exibir o nome da canção.

> A segunda coluna deve possuir o alias "reproducoes" e exibir a quantidade de pessoas que já escutaram a canção em questão.

> Seu resultado deve estar ordenado em ordem decrescente, baseando-se no número de reproduções. Em caso de empate, ordene os resultados pelo nome da canção em ordem alfabética. Queremos apenas o top 2 de músicas mais tocadas.

</p>
</details>

**6. Tendo como base o valor dos planos e o plano que cada pessoa usuária cadastrada possui no banco, queremos algumas informações sobre o faturamento da empresa. Crie uma QUERY que deve exibir quatro dados:**

<details><summary>Detalhes</summary>
<p>

> A primeira coluna deve ter o alias "faturamento_minimo" e exibir o menor valor de plano existente para uma pessoa usuária.

> A segunda coluna deve ter o alias "faturamento_maximo" e exibir o maior valor de plano existente para uma pessoa usuária.

> A terceira coluna deve ter o alias "faturamento_medio" e exibir o valor médio dos planos possuídos por pessoas usuárias até o momento.

> Por fim, a quarta coluna deve ter o alias "faturamento_total" e exibir o valor total obtido com os planos possuídos por pessoas usuárias.

> Para cada um desses dados, por se tratarem de valores monetários, deve-se arredondar o faturamento usando apenas duas casas decimais.

</p>
</details>

**7. Mostre uma relação de todos os álbuns produzidos por cada pessoa artista, ordenada pela quantidade de seguidores que ela possui, de acordo com os detalhes a seguir. Para tal, crie uma QUERY com as seguintes colunas:**

<details><summary>Detalhes</summary>
<p>

> A primeira coluna deve exibir o nome da pessoa artista, com o alias "artista".

> A segunda coluna deve exibir o nome do álbum, com o alias "album".

> A terceira coluna deve exibir a quantidade de pessoas seguidoras que aquela pessoa artista possui e deve possuir o alias "pessoas_seguidoras".

> Seus resultados devem estar ordenados de forma decrescente, baseando-se no número de pessoas seguidoras. Em caso de empate no número de pessoas, ordene os resultados pelo nome da pessoa artista em ordem alfabética e caso existam artistas com o mesmo nome, ordene os resultados pelo nome do álbum alfabeticamente.

</p>
</details>

**8. Mostre uma relação dos álbuns produzidos por uma pessoa artista específica, neste caso "Elis Regina". Para isto crie uma QUERY que o retorno deve exibir as seguintes colunas:**

<details><summary>Detalhes</summary>
<p>

> O nome da pessoa artista, com o alias "artista".

> O nome do álbum, com o alias "album".

> Os resultados devem ser ordenados pelo nome do álbum em ordem alfabética.

</p>
</details>

**9. Crie uma QUERY que exibe a quantidade de músicas que estão presentes atualmente no histórico de reprodução de uma pessoa usuária específica. Para este caso queremos saber quantas músicas estão no histórico da usuária "Barbara Liskov" e a consulta deve retornar a seguinte coluna:**

<details><summary>Detalhes</summary>
<p>

> O valor da quantidade, com o alias "musicas_no_historico".

</p>
</details>

REQUISITO BÔNUS

**10. Normalize a tabela da planilha SpotifyClone-fav-songs e crie uma tabela no banco de dados**

<details><summary>Detalhes</summary>
<p>

Seu banco de dados deve seguir as regras de negócio e ser capaz de recuperar:

> Informações sobre as canções favoritas das pessoas usuárias.
* Uma pessoa usuária pode possuir várias canções favoritas;
* Uma canção pode ser favoritada por várias pessoas usuárias.

</p>
</details>

**11. Crie uma QUERY que exibe o top 3 de álbuns com as músicas que mais foram favoritadas. O resultado deve possuir duas colunas:**

<details><summary>Detalhes</summary>
<p>

> album: O nome do álbum

> favoritadas: Quantas vezes as músicas do álbum foram favoritadas

> Seu resultado deve estar ordenado em ordem decrescente, baseando-se no número de favoritadas. Em caso de empate, ordene os resultados pelo nome do álbum em ordem alfabética. Queremos apenas o top 3 de álbuns com mais músicas favoritadas.

</p>
</details>

**12. Crie uma QUERY que exibe um ranking de artistas baseado na quantidade de favoritadas em suas músicas. O resultado deve possuir duas colunas:**

<details><summary>Detalhes</summary>
<p>

> artista: O nome da pessoa artista

> ranking: Uma classificação definida pela quantidade de favoritadas as canções da pessoa artista receberam.

> Seu resultado deve estar ordenado em ordem decrescente, baseando-se no número de favoritadas. Em caso de empate, ordene os resultados pelo nome da pessoa artista em ordem alfabética.

</p>
</details>

**13. Crie uma QUERY que exibe uma relação da quantidade total de pessoas usuárias e favoritadas por faixa etária. O resultado deve possuir três colunas:**

<details><summary>Detalhes</summary>
<p>

> faixa_etaria: A faixa etária das pessoas usuárias, sendo elas:
* Até 30 anos
* Entre 31 e 60 anos
* Maior de 60 anos

> total_pessoas_usuarias: O total de pessoas usuárias na respectiva faixa etária.

> total_favoritadas: O total de favoritadas realizadas pelas pessoas usuárias da respectiva faixa etária.

>  Seu resultado deve estar ordenado de acordo com a sequência das faixas etárias descritas acima.

</p>
</details>

## Sobre o curso da Trybe
O programa total de estudo conta com mais de 1.500 horas de aulas presenciais e online,divididas ao longo de 12 meses. O conteúdo aborda introdução ao desenvolvimento de software, front-end, back-end, ciência da computação, engenharia de software, metodologias ágeis e habilidades comportamentais.
