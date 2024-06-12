saldo = 1500
limite = 500
saque = 500

while True:

     sistema = input("Olá, seja bem vindo ao Banco Invest. Caso deseja realizar um saque, digite sacar ou se apenas deseja ver o seu saldo, digite saldo:")

     if sistema == 'sacar':
    
         valor = float(input("seu saldo equivale a 1500 reais, entretetanto apenas poderá sacar 500 reais hoje. informe o valor do saque:"))
         
         if valor > 500:
             print("impossivel realizar saque. limite para saque é de 500 reais.")
         
         else:
             saldo -= valor
             print(f"saque realizado com sucesso! seu novo saldo é de {saldo: .2f}")
             break  

     elif sistema == 'saldo':

        print(f"seu saldo equivale a {saldo}")
        break   
    
     else:
        print("operação desconhecida. tente novamente")
