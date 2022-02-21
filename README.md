






fun main() {
    
    var op = 11
   
   while (op != 0) {
    
        println("=======Escolha uma opção=========")
        println("1 - Cálculo de média: ")
        println("---------------------------------")
        println("2 - Verificar se é palíndroma: ")
        println("---------------------------------")
        println("3 - Sair: ")
        println("================================")
        
        var opcao = readLine()!!.toInt()

        if (opcao == 1) {
            println("Primeiro numero")
            var n1 = readLine()!!.toInt()
            println("Segundo numero")
            var n2 = readLine()!!.toInt()
            var rmedia = (n1 + n2) / 2

            println("A média é: 1${rmedia}")

        } else
            if (opcao == 2) {

                println("Palavra:")
                var palin = readLine()!!.toString()
                val reverso = palin.reversed()
                if (palin == reverso) {
                    println("é palindromo")
                } else if (palin != reverso) {
                    println("não palindromo")
                }

            } else
                if (opcao == 3) {
                    print("sair? 1 - sim 2 - não")
                var S = readLine()!!.toInt()
                    if (S== 1){
                        op = 0

                    } else {op = 4}


                         } else {
                        println("Opção inválida!!")
                    }
                }

}
