ALGORITMO "ContaMetrosCúbicos"

var
   tipo_consumidor:caracter
   conta:inteiro
   consumo, soma:real
   
inicio
   //Entrada de dados
   escreva("Digite sua conta: ")
   leia(conta)
   
   escreva("Digite seu tipo de consumidor (C, I ou R):")
   leia(tipo_consumidor)
   
   escolha (tipo_consumidor)
      caso "C"
         escreva("Digite seu consumo: ")
         leia(consumo)
         se consumo > 80 entao
            soma <- 500 + (0.25 * (consumo - 80))
            escreval("Conta: ", conta)
            escreva("Valor conta: " , soma)
         senao
            soma <- 500
            escreval("Conta: ", conta)
            escreva("Valor conta: " , soma)
         fimse
      caso "I"
         escreva("Digite seu consumo: ")
         leia(consumo)
         se consumo > 100 entao
            soma <- 800 + (0.04 * (consumo - 100))
            escreval("Conta: ", conta)
            escreva("Valor conta: " , soma)
         senao
            soma <- 800
            escreval("Conta: ", conta)
            escreva("Valor conta: " , soma)
         fimse
      caso "R"
         escreva("Digite seu consumo: ")
         leia(consumo)

         soma <- 5 + 0.05 * consumo
         
         escreval("Conta: ", conta)
         escreva("Valor conta: " , soma)
      outrocaso
         escreva("Escolha apenas entre C, I ou R!")
      fimescolha

fimalgoritmo
