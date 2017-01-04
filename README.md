# wildfly-swarm-enhanced-jax-rs-client-demo

WildFly Swarm Enhanced JAX-RS Client Demo

## Usage

### Build Apps

``` sh
./mvnw clean package
```

### Start addition service

``` sh
java -jar addition/target/addition-swarm.jar -Dswarm.http.port=8180
```

### Start  calc service

``` sh
java -jar calc/target/calc-swarm.jar 
```

### Access the Calc API

``` sh
$ curl 'localhost:8080?i1=10&i2=20'
{"result" : 30}⏎
```