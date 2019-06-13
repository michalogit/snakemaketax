# snakemaketax example

Here we simulate in a very simplified way processing of the tax declations. The snakemake workflow is run for every `*_a.txt` file in the `data` directory. To this file is added by concatenation another one with `*_a.txt` and placed in the folder `data_processed`. The report is packed in the envelope of the tax office `*_e.txt` file. Then, when all the final reports are produced in the `reports` folder, a marker file is produced for the completion of the work. 


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

