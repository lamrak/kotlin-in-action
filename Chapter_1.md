## Chapter 1:

**Kotlin basics**

- Classes declaration
- Functions declaration
- Variables declaration
- Control operators
- Cast
- Exceptions

_Classes declaration_

##### Function
```
fun max(a: Int, b: Int): Int {
    return if (a > b) a else b
}

fun main(args: Array<String>) {
    println(max(1, 2))
}
```
Ключевое слово `fun` `имя` (`параметры`) : `тип возвращаемого значения`.

`if`, `for`, `while` - выражения.

```
fun max(a: Int, b: Int): Int = if (a > b) a else b
```

##### Variables

`val` - immutable, final;
`var` - mutable

##### Classes

```
class Person(val name: String)
```

private value with public getter and setter

```
class Rectangle(val height: Int, val width: Int) {
   val square: Int
   get() = height * width;
}

fun main(args: Array<String>) {
    val rect = Rectangle(10, 5)
    println(rect.square)
}

```




