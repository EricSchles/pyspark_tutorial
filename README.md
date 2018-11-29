Running pyspark locally:

download pyspark locally: https://hub.docker.com/r/jupyter/pyspark-notebook/

via docker:

`docker pull jupyter/pyspark-notebook`

Then run:

`docker run -p 8889:8888 -v [replace with folder to save files]:/home/jovyan/work --rm --name jupyter jupyter/pyspark-notebook`


A Cheatsheet: 

https://www.qubole.com/resources/pyspark-cheatsheet/

Please note you need to do this:

```
from pyspark import SparkContext
from pyspark import SQLContext

sc = SparkContext()
sqlContext = SQLContext(sc)
```

Found here: https://www.analyticsvidhya.com/blog/2016/10/spark-dataframe-and-operations/

How to get the last row in pyspark:

```
expr = [last(col) for col in df.columns]
df.groupBy().agg(*expr).show()
```
