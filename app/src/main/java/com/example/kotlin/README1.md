# Key Syntax Rules

### Variables

1. val → Immutable (like final in Java)

2. var → Mutable

``` Kotlin
val speed = 100
var gear = 1
```

### Functions


``` Kotlin
fun sum(int a, int b): Int {
    return a+b
}
```

``` Kotlin
//single-expression function
fun sum(int a, int b) = a+b
```

### Null Safety

Nullable types: String?

Safe call: ?.

Elvis operator: ?:


``` Kotlin
var driverName: String? = null
println(driverName?.length ?: 0) // prints 0 if null
```

Non-null Assertion Operator: !!


### Strings interpolation

``` Kotlin
val mode = "Eco"
println("Current mode is $mode") 
```


### Control Flow

if / else

when → replacement for switch-case

Loops: for, while, do-while


### Collections

``` Kotlin
val sensors = listOf("Front", "Rear", "Left", "Right")
for(sensor in sensors) {
    println(sensor)
}
```

### Classes

``` Kotlin
class Car(val model: String, var speed: Int) {
    fun accelerate(amount: Int) {
        speed += amount
    }
}


val myCar = Car("Tesla", 60)
myCar.accelerate(10)
println(myCar.speed) // 70
```

| **Category**           | **Keywords**                                                                   | **Usage**                                     |
| ---------------------- | ------------------------------------------------------------------------------ | --------------------------------------------- |
| **Declaration**        | `val`, `var`, `fun`, `class`, `object`, `interface`, `const`                   | Define variables, functions, classes, objects |
| **OOP / Modifiers**    | `open`, `override`, `abstract`, `final`, `sealed`, `data`, `enum`, `companion` | Inheritance and class types                   |
| **Control Flow**       | `if`, `else`, `when`, `for`, `while`, `do`, `break`, `continue`, `return`      | Flow control                                  |
| **Null Safety**        | `null`, `is`, `as`, `as?`, `!!`, `?`, `in`, `!in`                              | Null handling, type checking, containment     |
| **Visibility / Scope** | `public`, `private`, `protected`, `internal`, `this`, `super`                  | Access modifiers                              |
| **Advanced**           | `by`, `get`, `set`, `typealias`, `where`, `suspend`, `yield`                   | Delegation, properties, generics, coroutines  |

