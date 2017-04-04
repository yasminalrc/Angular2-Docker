#API

## COMMON INFO
### URL
https://localhost:8443...

### STATUS
CODE | STATUS
---  | ---
200  | OK
201  | CREATED
304  | NOT MODIFIED
400  | BAD REQUEST
401  | UNAUTHORIZED - WRONG PASSWORD
404  | NOT FOUND


### LOGIN 
...URL              | METHOD    | INPUT                   | OUTPUT 
---                 | ---       | ---                     | --- 
/api/logIn          | ¿?        | None                    | User
/api/logOut         | ¿?        | HttpSession             | Boolean


### PRODUCTS
...URL              | METHOD    | INPUT                   | OUTPUT 
---                 | ---       | ---                     | --- 
/api/products/      | GET       | None                    | List of [Product]
/api/products/{id}  | GET       | Product.Id              | Product
/api/products/      | POST      | Product                 | Product 
/api/products/{id}  | PUT       | Product.Id, Product     | Product 
/api/products/{id}  | DELETE    | Product.Id              | Product 


### USERS
...URL              | METHOD    | INPUT                   | OUTPUT 
---                 | ---       | ---                     | --- 
/api/users/         | GET       | None                    | List of [User] 
/api/users/{id}     | GET       | User.Id                 | User
/api/users/         | POST      | User                    | User
/api/users/{id}     | PUT       | User.Id, Product        | User 
/api/users/{id}     | DELETE    | User.Id                 | User 


### ORDERS [Order = OrderSummary]
...URL              | METHOD    | INPUT                   | OUTPUT 
---                 | ---       | ---                     | --- 
/api/orders/        | GET       | None                    | List of [Order]               
/api/orders/{id}    | GET       | Order.Id                | Order     
/api/orders/        | POST      | Order                   | Order                     
/api/orders/{id}    | PUT       | Order.Id, Order         | Order    
/api/orders/{id}    | DELETE    | Order.Id                | Order    


#### Example of Product
https://localhost:8443/api/products/15
```json
{
  "id": 15,
  "name": "accesory15",
  "brand": "brand15",
  "model": "model15",
  "reference": "reference15",
  "type": "type3",
  "colour": null,
  "size": null,
  "sphere": null,
  "radio": null,
  "published": false,
  "price": 0.5,
  "quantity": 5,
  "image": "producto15",
  "description": "description15"
}
```