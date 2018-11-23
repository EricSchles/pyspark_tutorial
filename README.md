Running pyspark locally:

download pyspark locally: https://hub.docker.com/r/jupyter/pyspark-notebook/

via docker:

`docker pull jupyter/pyspark-notebook`

Then run:

`docker run -p 8889:8888 -v [replace with folder to save files]:/home/jovyan/work --rm --name jupyter jupyter/pyspark-notebook`


A Cheatsheet: 

https://www.qubole.com/resources/pyspark-cheatsheet/

