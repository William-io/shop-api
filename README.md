# shop-api
API/ASP.Net 5.0 + EFCORE 
//Dentro do Postman, Primeiro passo:
1. Criar uma categoria para incluir o produto.
    https://localhost:5001/v1/categories
    Usar o "POST", BODY, RAW, tipo JSON
        {
            "title":"Categoria 1"
        }

        {
            "title":""  //Sem a categoria no titulo vai ser aplicada a validação.
        }

2. Fazer um POST de products
    https://localhost:5001/v1/products
    Usar o "POST", BODY, RAW, tipo JSON
        {
            "title":"Produto 4",
            "description": "testando",
            "price": 1299,
            "categoryId": 1
        }

        {
            "title":"",   //Mais uma vez faz a validação
            "description": "testando",
            "price": 1299,
            "categoryId": 1
        }

3. Fazer um GET de products
    https://localhost:5001/v1/products
    //Vai lista todos os produtos da categoria.



