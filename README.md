
[![](https://images.microbadger.com/badges/image/thomasleduc/dynamodb-local.svg)](https://microbadger.com/images/thomasleduc/dynamodb-local)

## Build

To build :

```
docker build -t thomasleduc/dynamodb-local .
```

## Run
Runs the DynamoDB local service as a docker container. Run without parameters to see help:

```
docker run -i -t thomasleduc/dynamodb-local
```

Example:

```
docker run -i -t -p 7777:7777 thomasleduc/dynamodb-local -inMemory -port 7777
```

## Test

Assuming your dockerhost is `192.168.99.100` and you run the docker instance with `-port 7777` option. You can access to DynamoDB javascript shell by opening : 

```
192.168.99.100:7777/shell
```

