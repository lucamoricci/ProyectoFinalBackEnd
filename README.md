#Proyecto Final Curso BackEnd CoderHouse
#Alumno: Luca Moricci

+++++++++++++
Descripcion
+++++++++++++

El proyecto se consiste en el desarrollo del backend de un ecommerce en nodejs.
Para el desarrollo se han utilizados las siguiente librerias:

    express
    logger
    faker
    bcrypt
    commander
    mongo
    dotenv
    express-handlebars
    express-session
    mongoose
    mongoose-paginate-v2
    nodemailer
    passport
    passport-github2
    passport-local
    socket.io
    swagger-jsdoc
    winston


+++++++++++++++++++
Consideraciones:
+++++++++++++++++++

Estan desarrollados todos los endpoints solicitados.

A cada usuario se le asigna un carrito al momento del alta.

Si bien la implmentacion en archivos no esta completa, deje la deficion de la factory para tenerlo.

Estan desarrollados todas los endpoints solicitados para productos, carrito y usuarios.

El contenido de las variables de entorno, no estan en github y se incluyen al final de este archivo.

El chat no lo puse ya que no estaba como parte de las entregas obligatorias, la fucionalidad de sockets esta implementada para la vista realtime y para no demorar la entrega fundamentalmente .




## Proceso de Compra - API Reference 

#### Login

```http
  GET /login
```
Permite loguerse, registrar un usuario nuevo y restablecer contraseña.


#### Products

```http
  GET /productos
```
Permite ver los productos cargados en el base de datos y agregarlos al carrito de cada usuario.

#### Real Time Products 

```http
  GET /realtimeproducts
```
se pueden ver en tiempo real los productos cargados. Se pueden eliminar y cargar nuevos productos como admin.

#### Purchase preview 

```http
  GET /api/carrito/${cartid}/purchase_preview
```
Vista preliminar de los productos que estaria comprando un usuario/carrito (profile: user)

#### Purchase

```http
  GET /api/carrito/${cartid}/purchase
```
Cierra la compra, calcula total, descuenta stock, deja en el carrito prods sin stock al momento de confirmar.

#### Users List

```http
  GET /users
```
Muestra lista de usuarios y permite cambiar el rol (profile: admin)






