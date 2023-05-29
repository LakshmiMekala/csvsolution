# Run CSVServer

## Part I

* Generate the inputfile with gencsv.sh file
```
    ./gencsv.sh <start-index> <end-index>
```

* Now use the generated input file and run the docker command

```
docker run -it -p 9393:9300 -e CSVSERVER_BORDER=Orange  -v $(pwd)/inputdata/inputFile:/csvserver/inputdata  infracloudio/csvserver:latest
```
* Try accessing the application on 

```
http://localhost:9300
```

## Part II

* Run the csvserver application with docker-compose

```
docker-compose up
```

* Try accessing the application on 

```
http://localhost:9300
```

## Part III