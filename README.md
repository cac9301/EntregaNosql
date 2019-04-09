# bases-nosql


     CARLOS ARTURO CARMONA LARROTTA 1532083-2711





```bash
-docker exec -it bcecf67ca725  
mongoimport -d EntregaNosql -c mydbcoll --file /path/to/file --jsonArray

-docker exec 94b5bbaf5f57 mongoimport -d CancerBD --collection cancerTotal --file/tmp/tem2.json --jsonarray
```
## las consultas en la base de datos que se realizan para verificar que se hizo

hacemos consultas en la base de datos para comprobar que todo funciona bien por ejemplo:

-consulta total de articulos
```bash
-db.mydbcoll.count()
```
retorno 2500 que corresponde a todos los registros 

-consulta total articulos año 2019
```bash
-db.mydbcoll.count({"year": 2019}).count()
```
retorno 2499 articulos (habia un articulo que le cambiamos la fecha en el json para comprobar que este bien
