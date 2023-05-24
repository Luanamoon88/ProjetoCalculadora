# Olá, esse projeto simula uma calculadora
import math

print("Calculadora Uninove")
print()
print("- Para prosseguir, informe a opção desejada:")
print()
print("1. Adição")
print("2. Subtração")
print("3. Multiplicação")
print("4. Divisão (Resto de Divisão)")
print("5. Divisão")
print("6. Raíz Quadrada (Somente um Número de Entrada)")
print("7. Exponenciação")
print()
operacao = input("Escolha a operação desejada: ") 

if operacao in ['1','2','3','4','5','6','7']:
  numero1 = float(input("Digite o 1º número: "))
else:
  print("Dados Inconsistente!")
print()
if operacao != '6':
    numero2 = float(input("Digite o 2º número: "))

if operacao == '1':
    resultado = numero1 + numero2
    print("Resultado:", resultado)
elif operacao == '2':
    resultado = numero1 - numero2
    print("Resultado:", resultado)
elif operacao == '3':
    resultado = numero1 * numero2
    print("Resultado:", resultado)
elif operacao == '4':
    resultado = numero1 % numero2
    print("Resultado:", resultado)
elif operacao == '5':
    if numero2 != 0:
        resultado = numero1 / numero2
        print("Resultado:", resultado)
    else:
        print("Dados inconsistentes. Divisão por zero não é permitida.")
elif operacao == '6':
  if numero1>=0:
    resultado = math.sqrt(numero1)
    print("Resultado:", resultado)
  else:
    print("Dados Inconsistentes")
elif operacao == '7':
    resultado = numero1 ** numero2
    print("Resultado:", resultado)
else:
    print("Dados inconsistentes. Opção inválida.")
