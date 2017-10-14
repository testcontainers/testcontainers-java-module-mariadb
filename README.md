# TestContainers MariaDB Module [![Build Status](https://travis-ci.org/testcontainers/testcontainers-java-module-mariadb.svg?branch=master)](https://travis-ci.org/testcontainers/testcontainers-java-module-mariadb)

Testcontainers module for the MariaDB database.

See [testcontainers.org](https://www.testcontainers.org) for more information about Testcontainers.

<!--[![Build Status](https://travis-ci.org/testcontainers/testcontainers-java.svg?branch=master)](https://travis-ci.org/testcontainers/testcontainers-java)-->

## Usage example

Running MariaDB as a stand-in for in a test:

```java
public class SomeTest {

    @Rule
    public MariaDBContainer mariaDB = new MariaDBContainer();
    
    @Test
    public void someTestMethod() {
        String url = mariaDB.getJdbcUrl();

        ... create a connection and run test as normal
```

## Dependency information

### Maven

```
<dependency>
    <groupId>org.testcontainers</groupId>
    <artifactId>mariadb</artifactId>
    <version>1.4.3</version>
</dependency>
```

### Gradle

```
compile group: 'org.testcontainers', name: 'mariadb', version: '1.4.3'
```


## License

See [LICENSE](LICENSE).

## Copyright

Copyright (c) 2015 - 2017 Richard North and other authors.

See [AUTHORS](AUTHORS) for contributors.
