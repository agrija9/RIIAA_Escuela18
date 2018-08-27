### RIIAA Escuela18

Repo para la escuela de verano de la RIIAA 2018


#### Requisitos

1. Laptop con Mozilla Firefox o Google Chrome.
2. [Python 3.6 (anaconda)](https://www.anaconda.com/download/)
3. Un ambiente python con varios paquetes instalados. Estos paquetes están descritos dentro de `requirements.txt` o `environment.yml`.


### Con Anaconda: Crear un conda environment

Desde una terminal, estando en la carpeta donde se encuentra **environment.yml**, corres el comando:
```
conda env create -f environment.yml
```

### Con pip
Desde una terminal, estando en la carpeta donde se encuentra **requirements.txt**, corres el comando:
```
pip install -r requirements.txt
```

### Con Docker
Puedes construir una imagen docker, es decir un ambiente virtual via el siguiente comando
```
docker build -t "riiaa18" .
```
y luego para correr el ambiente docker en la carpeta favorita de tu eleccion usas el comando
```
docker run -it --rm -p 8890:8888 -v $(pwd):/home/jovyan/work  riiaa18
```
