# Run CSVServer

## Part 1

* Generate the inputfile with gencsv.sh file
```
    ./gencsv.sh <start-index> <end-index>
```

* Now use the generated input file and run the docker command

```
docker run -it -p 9393:9300 -e CSVSERVER_BORDER=Orange  -v $(pwd)/inputdata/inputFile:/csvserver/inputdata  infracloudio/csvserver:latest
```

## Part 2


## Part 3