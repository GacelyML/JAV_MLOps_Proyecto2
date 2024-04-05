# Proyecto 2: MLOps

## Por Brayan Carvajal, Juan Pablo Nieto y Nicolás Rojas

blablabla

## Ejecución del código

El código en este repositorio puede ejecutarse siguiendo los siguientes pasos:

- Instale docker siguiendo las instrucciones en la [documentación oficial](https://docs.docker.com/get-docker/).
- Clone este repositorio con el siguiente comando:
    ```shell
    git clone https://github.com/GacelyML/JAV_MLOps_Proyecto2
    ```
- Ubíquese en la carpeta recién creada:
    ```shell
    cd JAV_MLOps_Proyecto2
    ```
- Abra en una nueva pestaña una terminal dentro del entorno Jupyter y descargue los datos a través de los siguientes comandos:
    ```shell
    dvc remote modify --local data credentialpath './credentials/test-gcp-gacelydev-e4bc89448148.json'
    ```
    ```shell
    dvc pull
    ```
- Cree los servicios con el siguiente comando:
    ```shell
    docker compose up
    ```
- Al finalizar la creación del servicio, en la consola se obtendrá un token de acceso que permitirá ingresar desde un navegador web en xxx
- Ingrese a Jupyterlab desde la interfaz web y desde ahí abra el notebook [model.ipynb](notebooks/model.ipynb).

docker compose down --volumes --remove-orphans