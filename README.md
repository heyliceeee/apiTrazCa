# API da app "Traz Cá"
## Produto

<details>
  <summary>Criar</summary>
  <pre> Insere dados de um produto em formato JSON. </pre>
  
* **URL**

  /insertProduct

* **Método:**

  `POST`
  
*  **Parâmetros de URL**

   Nenhum

* **Parâmetros de dados**

  **Obrigatório:**
 
   `name=[string]`
   `price=[decimal]`
   `category=[string]`
   `idRestaurant=[integer]`
   
   
   **Opcional:**
 
   `description=[string]`
   `image=[string]`
   `nStars=[integer]`
   `allergens=[string]`
   `mainIngredients=[string]`
   `nutritionalValue=[string]`

* **Resposta de sucesso:**

  * **StatusCode:** 200 <br />
    **Message:** `{ "Produto criado com sucesso" }`
 
* **Resposta de erro:**

  * **StatusCode:** 404 <br />
    **Message:** `{ motivo do erro }`

  OU

  * **StatusCode:** 404 <br />
    **Message:** `{ "Produto criado sem sucesso" }`
</details>


## Pedido

<details>
  <summary>Criar</summary>
  <pre> Insere dados de um pedido em formato JSON. </pre>
  
* **URL**

  /insertOrder

* **Método:**

  `POST`
  
*  **Parâmetros de URL**

   Nenhum

* **Parâmetros de dados**

  **Obrigatório:**
 
   `timeUserAddress=[datetime]`
   `idCart=[integer]`

* **Resposta de sucesso:**

  * **StatusCode:** 200 <br />
    **Message:** `{ "Pedido criado com sucesso" }`
 
* **Resposta de erro:**

  * **StatusCode:** 404 <br />
    **Message:** `{ motivo do erro }`

  OU

  * **StatusCode:** 404 <br />
    **Message:** `{ "Pedido criado sem sucesso" }`
</details>


## Carrinho

<details>
  <summary>Criar</summary>
  <pre> Insere dados de um carrinho em formato JSON. </pre>
  
* **URL**

  /insertCart

* **Método:**

  `POST`
  
*  **Parâmetros de URL**

   Nenhum

* **Parâmetros de dados**

  **Obrigatório:**
 
   `subtotal=[decimal]`
   `deliveryFee=[decimal]`
   `discount=[decimal]`
   `total=[decimal]`
   `idUser=[integer]`

* **Resposta de sucesso:**

  * **StatusCode:** 200 <br />
    **Message:** `{ "Carrinho criado com sucesso" }`
 
* **Resposta de erro:**

  * **StatusCode:** 404 <br />
    **Message:** `{ motivo do erro }`

  OU

  * **StatusCode:** 404 <br />
    **Message:** `{ "Carrinho criado sem sucesso" }`
</details>


## Item do Carrinho

<details>
  <summary>Criar</summary>
  <pre> Insere dados de um item do carrinho em formato JSON. </pre>
  
* **URL**

  /insertCartItem

* **Método:**

  `POST`
  
*  **Parâmetros de URL**

   Nenhum

* **Parâmetros de dados**

  **Obrigatório:**
 
   `quantity=[integer]`
   `idProduct=[integer]`
   `idCart=[integer]`
   
   
   **Opcional:**
 
   `noteProduct=[string]`

* **Resposta de sucesso:**

  * **StatusCode:** 200 <br />
    **Message:** `{ "Item do carrinho criado com sucesso" }`
 
* **Resposta de erro:**

  * **StatusCode:** 404 <br />
    **Message:** `{ motivo do erro }`

  OU

  * **StatusCode:** 404 <br />
    **Message:** `{ "Item do carrinho criado sem sucesso" }`
</details>


## Comentário acerca do Produto

<details>
  <summary>Criar</summary>
  <pre> Insere dados de um comentário acerca de um produto em formato JSON. </pre>
  
* **URL**

  /insertCommentProduct

* **Método:**

  `POST`
  
*  **Parâmetros de URL**

   Nenhum

* **Parâmetros de dados**

  **Obrigatório:**
 
   `nameClient=[string]`
   `idProduct=[integer]`
   
   
   **Opcional:**
 
   `image=[string]`
   `nStars=[integer]`
   `text=[string]`

* **Resposta de sucesso:**

  * **StatusCode:** 200 <br />
    **Message:** `{ "Comentário criado com sucesso" }`
 
* **Resposta de erro:**

  * **StatusCode:** 404 <br />
    **Message:** `{ motivo do erro }`

  OU

  * **StatusCode:** 404 <br />
    **Message:** `{ "Comentário criado sem sucesso" }`
</details>


## Comentário acerca do Trabalhador

<details>
  <summary>Criar</summary>
  <pre> Insere dados de um comentário acerca de um trabalhador em formato JSON. </pre>
  
* **URL**

  /insertCommentWorker

* **Método:**

  `POST`
  
*  **Parâmetros de URL**

   Nenhum

* **Parâmetros de dados**

  **Obrigatório:**
 
   `nameClient=[string]`
   `idWorker=[integer]`
   
   
   **Opcional:**
 
   `image=[string]`
   `nStars=[integer]`
   `text=[string]`

* **Resposta de sucesso:**

  * **StatusCode:** 200 <br />
    **Message:** `{ "Comentário criado com sucesso" }`
 
* **Resposta de erro:**

  * **StatusCode:** 404 <br />
    **Message:** `{ motivo do erro }`

  OU

  * **StatusCode:** 404 <br />
    **Message:** `{ "Comentário criado sem sucesso" }`
</details>


## Restaurante

<details>
  <summary>Criar</summary>
  <pre> Insere dados de um restaurante em formato JSON. </pre>
  
* **URL**

  /insertRestaurant

* **Método:**

  `POST`
  
*  **Parâmetros de URL**

   Nenhum

* **Parâmetros de dados**

  **Obrigatório:**
 
   `name=[string]`
   `address=[string]`
   
   
   **Opcional:**
 
   `image=[string]`
   `nStars=[integer]`
   `allCategories=[string]`
   `cheapPriceProduct=[integer]`
   `distanceUserAddress=[integer]`
   `description=[string]`

* **Resposta de sucesso:**

  * **StatusCode:** 200 <br />
    **Message:** `{ "Restaurante criado com sucesso" }`
 
* **Resposta de erro:**

  * **StatusCode:** 404 <br />
    **Message:** `{ motivo do erro }`

  OU

  * **StatusCode:** 404 <br />
    **Message:** `{ "Restaurante criado sem sucesso" }`
</details>




## Utilizador
    
<details>
  <summary>Criar</summary>
  <pre> Insere dados de um utilizador em formato JSON. </pre>
  
* **URL**

  /insertUser

* **Método:**

  `POST`
  
*  **Parâmetros de URL**

   Nenhum

* **Parâmetros de dados**

  **Obrigatório:**
 
   `name=[string]`
   `role=[string]`
   `address=[string]`
   `email=[string]`
   `password=[string]`
   `paypal=[string]`
   
   
   **Opcional:**
 
   `phoneNumber=[string]`

* **Resposta de sucesso:**

  * **StatusCode:** 200 <br />
    **Message:** `{ "Utilizador criado com sucesso" }`
 
* **Resposta de erro:**

  * **StatusCode:** 404 <br />
    **Message:** `{ motivo do erro }`

  OU

  * **StatusCode:** 404 <br />
    **Message:** `{ "Utilizador criado sem sucesso" }`
</details>



## Log
    
<details>
  <summary>Criar</summary>
  <pre> Insere dados de uma log em formato JSON. </pre>
  
* **URL**

  /insertLog

* **Método:**

  `POST`
  
*  **Parâmetros de URL**

   Nenhum

* **Parâmetros de dados**

  **Obrigatório:**
 
   `dateTime=[dateTime]`
   `idUser=[integer]`
   `type=[string]`
   `titleLog=[string]`
   
   **Opcional:**
 
   `resume=[string]`

* **Resposta de sucesso:**

  * **StatusCode:** 200 <br />
    **Message:** `{ "Log criada com sucesso" }`
 
* **Resposta de erro:**

  * **StatusCode:** 404 <br />
    **Message:** `{ motivo do erro }`

  OU

  * **StatusCode:** 404 <br />
    **Message:** `{ "Log criada sem sucesso" }`
</details>
