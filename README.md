# Projeto MySQL All For One
## Este repositório contém o desenvolvimento do meu 18º projeto na Trybe

Chegou o momento de ter o primeiro contato com banco de dados e, na Trybe, utilizamos o MySQL como banco relacional. Neste projeto Al For One, eu pude colocar em prática os conceitos básicos aprendidos sobre o assunto. Sendo assim, foi um projeto bem bacana de ser desenvolvido.   

## Detalhes do projeto

Confira os requisitos exigidos pela Trybe (texto extraído dos readme oficial da Trybe):

**1. Exiba apenas os nomes dos produtos na tabela products**

---

**2. Exiba os dados de todas as colunas da tabela products**

---

**3. Escreva uma query que exiba os valores da coluna que representa a primary key da tabela products**

---

**4. Conte quantos registros existem na coluna product_name da tabela products**

---

**5. Monte uma query que exiba os dados da tabela products a partir do quarto registro até o décimo terceiro**

---

**6. Exiba os dados das colunas product_name e id da tabela products de maneira que os resultados estejam em ordem alfabética dos nomes**

---

**7. Mostre apenas os ids dos 5 últimos registros da tabela products (a ordenação deve ser baseada na coluna id)**

---

**8.  Faça uma consulta na tabela employees que retorne o nome completo da pessoa colaboradora (colunas first_name e last_name) com o nome full_name e também a localização completa (colunas city, state_province e address) com o nome location**

---

**9. Mostre todos os valores de notes da tabela purchase_orders que não são nulos**

---

**10. Mostre todos os dados da tabela purchase_orders em ordem decrescente, ordenados por created_by em que o created_by é maior ou igual a 3**

<details><summary>Detalhes</summary>
<p>

> Ordene também os resultados pelo id de forma crescente, como critério de desempate para a ordenação.

</p>
</details>

---

**11. Exiba os dados da coluna notes da tabela purchase_orders em que seu valor de Purchase generated based on Order é maior ou igual a 30 e menor ou igual a 39**

---

**12. Mostre as submitted_date de purchase_orders em que a submitted_date é do dia 26 de abril de 2006**

---

**13. Mostre o supplier_id das purchase_orders em que o supplier_id seja 1 ou 3**

---

**14. Mostre os resultados da coluna supplier_id da tabela purchase_orders em que o supplier_id seja maior ou igual a 1 e menor ou igual 3**

---

**15. Mostre somente as horas (sem os minutos e os segundos) da coluna submitted_date de todos registros da tabela purchase_orders**

<details><summary>Detalhes</summary>
<p>

> No resultado, a hora extraída da coluna submitted_date deve ser chamada de submitted_hour.

</p>
</details>

---

**16. Exiba a submitted_date das purchase_orders que estão entre 2006-01-26 00:00:00 e 2006-03-31 23:59:59**

---

**17. Mostre os registros das colunas id e supplier_id das purchase_orders em que os supplier_id sejam tanto 1, ou 3, ou 5, ou 7**

---

**18. Mostre todos os registros de purchase_orders que tem o supplier_id igual a 3 e status_id igual a 2**

---

**19. Mostre a quantidade de pedidos que foram feitos na tabela orders pelo employee_id igual a 5 ou 6, e que foram enviados através do método(coluna) shipper_id igual a 2**

<details><summary>Detalhes</summary>
<p>

> No resultado, a coluna que contém a contagem de pedidos deve ser chamada de orders_count.

</p>
</details>

---

**20. Adicione à tabela order_details um registro com order_id: 69, product_id: 80, quantity: 15.0000, unit_price: 15.0000, discount: 0, status_id: 2, date_allocated: NULL, purchase_order_id: NULL e inventory_id: 129**

---

**21. Adicione com um único INSERT, duas linhas à tabela order_details com os mesmos dados do requisito 20**

---

**22. Atualize todos os dados da coluna discount, na tabela order_details, para 15**

---

**23. Atualize os dados da coluna discount da tabela order_details para 30, onde o valor na coluna unit_price seja menor que 10.0000**

---

**24. Atualize os dados da coluna discount da tabela order_details para 45, onde o valor na coluna unit_price seja maior que 10.0000 e o id seja um número entre 30 e 40**

---

**25. Delete todos os dados em que a unit_price da tabela order_details seja menor que 10.0000**

---

**26. Delete todos os dados em que a unit_price da tabela order_details seja maior que 10.0000**

---

**27. Delete todos os dados da tabela order_details**

---

## Sobre o curso da Trybe
O programa total de estudo conta com mais de 1.500 horas de aulas presenciais e online,divididas ao longo de 12 meses. O conteúdo aborda introdução ao desenvolvimento de software, front-end, back-end, ciência da computação, engenharia de software, metodologias ágeis e habilidades comportamentais.
