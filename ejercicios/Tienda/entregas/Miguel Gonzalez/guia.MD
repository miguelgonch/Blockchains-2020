# Instrucciones de uso

## Configuración del ambiente
En este caso se utilizo Flask de python como servidor web para facilitar la creación del gui, por lo que se debe de instalar utilizando el siguiente comando:
```
pip install flask
```

## Configuración de la aplicación
Para poder utilizar la aplicación se debe de hacer deploy del contrato "Registros.sol" e ingresar la dirección del contrato en ./app/app.py en el campo "addressRegistro". Si es necesario se puede cambiar la dirección del blockchain modificando el campo bchainAddress

Una vez instalado flask y configurado el contro se ejecuta el python script ./app/app.py y se abre el explorador en http://127.0.0.1:5000/ (Este servidor es montado automaticamente por Flask).

## Rutas dentro de la aplicación
* http://127.0.0.1:5000/: Lleva a la página inicial del sitio para realizar una búsqueda del dominio
* http://127.0.0.1:5000/hosts: Lleva a la página en donde se muestra el listado de dominios registrados y las ofertas existentes

## Para imprimir archivo hosts
En la pagina http://127.0.0.1:5000/hosts del sitio hacer click en el botón de "Click to Save" y escoger en donde guardar el archivo

## Para aceptar ofertas
Esta función no fue implementada en el gui. Es posible aceptar las ofertas utilizando la dirección del contrato oferta (mostrado en la pagina http://127.0.0.1:5000/hosts) ingresándolo manualmente en el blockchain.
