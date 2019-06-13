# snakemaketax example

Install the minimal snakemake in your environment with conda

```
conda install -c bioconda -c conda-forge snakemake-minimal
```

Clone the exercise repo

```
https://github.com/michalogit/snakemaketax.git
```

Use the simple processing

```
cp Snakefile1 Snakefile
```

Do the dry run


```
snakemake -np
```

and the real run 

```
snakemake -p
```


you can produce the graph too

```
snakemake --dag > graph1.dag
```


![graph1](https://github.com/michalogit/snakemaketax/blob/master/graphs/graph1.png "Simple workflow")

The same exercise with the more complex Snakefile

```
cp Snakefile2 Snakefile
```


![graph2](https://github.com/michalogit/snakemaketax/blob/master/graphs/graph2.png "More complex workflow")

