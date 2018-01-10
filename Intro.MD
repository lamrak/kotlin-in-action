## Intro

- Review
- Main points
- Differences with other languages 
- Simple program

Kotlin is a statically-typed programming language that runs on the JVM.

Kotlin позволяет использовать функциональный стиль программирования, но не требует этого. Например:
- lambda
- передача функции как аргумент
- создавать неизменяеммые обьекты
- набор инструментов для работы со стандартными коллекциями и библиотека в функциональном стиле.

Kotlin
- Прагматичен - практический язык для решения реальных задач.
- Лаконичен - язык не содержит избыточного кода
- Безопасен - дизайн предотвращает появления ошибок в программе
```
val s: String? = null //can be null
val s: String = ""    //can't be null
```

```
if (val is String)
  val.trim()
```
- Совместим с Java

Kotlin компилируется в *.class так же как и Java

Пример программы:

```
data class Person(val name: String, val age: Int? = null)

fun main(args: Array<String>) {
    val persons = listOf(Person("Alice"), Person("Bob", age = 29))

    val oldest = persons.maxBy { it.age ?: 0 }
    
    println("The oldest is: $oldest")
}

// The oldest is: Person(name=Bob, age=29)
```
