# Configuration

## Spring Boot

It's easy to integrate Kotlin and Spring Boot.

For example: [Creating a RESTful Web Service with Spring Boot](https://kotlinlang.org/docs/tutorials/spring-boot-restful.html)

We have 2 things to do:
1. Change `build.gradle`
2. Create a class `Application` to launch Spring Boot

### build.gradle

Add an element in `buildscript.dependencies` for spring Boot:

```
classpath "org.springframework.boot:spring-boot-gradle-plugin:1.3.0.RELEASE"
```

And another one in `dependencies`:

```
compile 'org.springframework.boot:spring-boot-starter-web'
```

### Application.kt

Create a file named `Application.kt` in `src/main/kotlin/fr/xebia/xke-kotlin/` and create an [open class](https://kotlinlang.org/docs/reference/classes.html#inheritance) (Spring boot @Configuration classes cannot be final) annotaded with `@SpringBootApplication`.

Spring Boot looks for a **public static main method**, we need to define this in Kotlin using the @JvmStatic annotation. For this, we create a companion object inside where we can then create a function annotated with @JvmStatic.

That's it we have configured Kotlin and Spring Boot !

## Jackson

Spring looks for a `@Bean` returning a `Jackson2ObjectMapperBuilder` object so we need to declare a function returning that kind of class.

For that we can use the builder `Jackson2ObjectMapperBuilder()`.

Finally we need to install 2 modules with Jackson:
* KotlinModule() : so we can use [Data class](https://kotlinlang.org/docs/reference/data-classes.html) with Jackson
* JavaTimeModule() : so we can serialize/deserialize Java 8 Date

:warning: You need to add the following `dependencies` in `build.gradle`:

```
compile 'com.fasterxml.jackson.module:jackson-module-kotlin:2.6.5-2'
compile 'com.fasterxml.jackson.datatype:jackson-datatype-jsr310:2.6.1'
```

Previous: [Project Creation](01_CreateProject.md)
Next: [Spring Boot Configuration](03_AddDataClass.md)

:horse:
