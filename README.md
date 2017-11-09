## Nodos 

Cliente: manejo de los clientes(Cine planeta, Cine Stark, CinePapaya)

**Api Gateway** : es una capa abstracta que impide a los usuarios 
ver la existencia de los micro servicios facilitando la comunicacion con
los usuarios, se esta usando bastante apis por ello es necesario usar
api gateway para facilitar todo. Contiene API Service Management para 
gestionar servicios entrantes y Traffic Manager para mejorar rendimiento 
y disponibilidad.

**Event sourcing** : se mantendra una lista de todas las transacciones que
ocurierron y van a ocurrir guardando la fecha y hora en que se genero
ademas tambien se guardara el nombre de la persona que realizo la transaccion
al igual que el numero de entradas que esta persona compro

* BD: Mantiene toda informacion de Cine Planeta
* BD: Mantiene toda informacion de Cine Stark
* BD: Mantiene toda informacion de Cine Papaya

* Funciones:se utiliza para ver la informacion las funciones
* Compra:Se utiliza para ver la informacion de las compras 
* Cine: Se utiliza para ver la informacion de los cines disponibles
* Ticket: se utiliza para ver la informacion de los tickets
* Cartelera: utilizado para ver las peliculas disponibles en todos los cines
* Pelicula: utilizado para ver las peliculas disponibles
* Analitica: servicio de analitica de la empresa
* Server BI: Motor OLAP para analitica

---

## Componentes

**Todos los Apis se dividiran en comandos y consultas siguiendo CQSR**
* Api funcion
* Api Compra
* Api Cine
* Api Ticket
* Api Cartelera
* Api Pelicula
* Api Analitica
