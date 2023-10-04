# Praticando Kotlin no Playground

### Imprimindo uma mensagem "olá Mundo"

```
package org.kotlinlang.play         // Definição do pacote

fun main() {                        // ponto de entrada de código kotrin, definido pela função [main]
    println("Hello, World!")        // imprime na saida padrão um texto, pulando uma linha logo em seguida
}
```
### Funções - Valores de Parâmetro Padrão e Argumentos Nomeados

```
fun printMessage(message: String): Unit {                               // 1
    println(message)
}

fun printMessageWithPrefix(message: String, prefix: String = "Info") {  // 2
    println("[$prefix] $message")
}

fun sum(x: Int, y: Int): Int {                                          // 3
    return x + y
}

fun multiply(x: Int, y: Int) = x * y                                    // 4

fun main() {
    printMessage("Hello")                                               // 5                    
    printMessageWithPrefix("Hello", "Log")                              // 6
    printMessageWithPrefix("Hello")                                     // 7
    printMessageWithPrefix(prefix = "Log", message = "Hello")           // 8
    println(sum(1, 2))                                                  // 9
    println(multiply(2, 4))                                             // 10
}

```