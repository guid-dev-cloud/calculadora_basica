# calculadora_basica
Calculadora básica para atividade em curso de Analista de dados

continuar = 's'
while continuar == 's':

  num1 = input("Digite o primeiro número: ")
  num2 = input("Digite o segundo número: ")

  num1 = float(num1)
  num2 = float(num2)

  print("\nEscolha uma opção para calcular:")
  print("1 - Soma | 2 - Subtração | 3 - Multiplicação | 4 - Divisão")

  opcao = input("\nDigite o número da opção desejada (1/2/3/4): ")

  if opcao == '1':
      resultado = num1 + num2
      print(f"Resultado da Soma: {resultado}")
  elif opcao == '2':
      resultado = num1 - num2
      print(f"Resultado da Subtração: {resultado}")
  elif opcao == '3':
      resultado = num1 * num2
      print(f"Resultado da Multiplicação: {resultado}")
  elif opcao == '4':
      if num2 != 0:
          resultado = num1 / num2
          print(f"Resultado da Divisão: {resultado}")
      else:
          print("Erro: Não é possível dividir por zero!")
  else:
      print("Opção inválida!")

  continuar = input("\nDeseja realizar um novo cálculo? Digite: s (para sim) ou n (para não): ")

print("\nCalculadora encerrada!")
