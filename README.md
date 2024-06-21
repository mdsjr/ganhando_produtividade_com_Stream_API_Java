# Bootcamp DIO Santander Java

![Bootcamp](https://example.com/bootcamp-banner.png)

Repositório criado para acompanhar o Bootcamp DIO Santander Java. Este repositório contém exemplos e exercícios relacionados aos conceitos de programação abordados durante o Bootcamp.

## Índice

1. [Conhecendo as Funcionalidades](#conhecendo-as-funcionalidades)
2. [Programação Imperativa vs. Programação Declarativa](#programação-imperativa-vs-programação-declarativa)
3. [Lambda Expressions](#lambda-expressions)
4. [Method Reference](#method-reference)
5. [Functional Interface](#functional-interface)
    - [Consumer\<T\>](#consumer-t)
    - [Function\<T,R\>](#function-tr)
    - [Predicate\<T\>](#predicate-t)
6. [Operações do Stream API](#operações-do-stream-api)
7. [Utilizando a Classe Optional\<T\>](#utilizando-a-classe-optional-t)

---

## Conhecendo as Funcionalidades

Explore as funcionalidades principais do Java, compreendendo a diferença entre a programação imperativa e a declarativa.

## Programação Imperativa vs. Programação Declarativa

Entenda as diferenças e aplique os conceitos de programação imperativa e declarativa em seus projetos.

## Lambda Expressions

Aprenda a utilizar expressões lambda para tornar seu código mais conciso e legível.

```java
// Exemplo de Lambda Expression
List<String> names = Arrays.asList("Ana", "Pedro", "João");
names.forEach(name -> System.out.println(name));
```
## Method Reference
Utilize referências a métodos para simplificar ainda mais seu código.
```
// Exemplo de Method Reference
names.forEach(System.out::println);
```

## Functional Interface
### Consumer <T<T>>
A interface Consumer aceita um único argumento e não retorna nenhum resultado.

```
Consumer<String> print = System.out::println;
print.accept("Hello, World!");
```
## Function<T,R>
A interface Function aceita um argumento e produz um resultado.
```
Function<String, Integer> length = String::length;
System.out.println(length.apply("Hello"));
```

## Predicate<T>
A interface Predicate representa uma função que testa uma condição sobre um argumento.
```
Predicate<String> isEmpty = String::isEmpty;
System.out.println(isEmpty.test("Hello"));

```
## Operações do Stream API
Conheça e utilize as operações da Stream API para processar coleções de forma funcional.
```
List<String> filteredNames = names.stream()
                                   .filter(name -> name.startsWith("A"))
                                   .collect(Collectors.toList());
System.out.println(filteredNames);
```
## Utilizando a Classe Optional<T>
Evite NullPointerExceptions utilizando a classe Optional.
````
Optional<String> optionalName = Optional.of("Ana");
optionalName.ifPresent(System.out::println);

````

## Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.

## Licença
Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE para mais detalhes.


