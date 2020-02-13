
# Spring Boot with H2
https://howtodoinjava.com/spring-boot2/h2-database-example/

## Add below properties in application.properties

### Inmemory based DB
```
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=arvind
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
```
### File based DB 
```
spring.datasource.url=jdbc:h2:~/testdb
```

#### Pleae find the list of important hibernate annotations:-

https://www.journaldev.com/17803/jpa-hibernate-annotations

* @Embeddable
* @EmbeddedId
* @Id
* @Entity
* @Table
* @Column
* @ElementCollection
* @IdClass
* @OneToOne



#### @Id is mandatory. Is it possible to create entity class without @Id 

Spring Data JPA does not allow to create JPA entity class without @Id, as it is as per JPA specification

<a href="https://github.com/arvindekka/SpringDataJPA-Hibernate/blob/master/JavaPersistence.pdf">See section 2.4 of the JPA specification. </a>

