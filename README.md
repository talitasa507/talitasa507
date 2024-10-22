- 👋 Hi, I’m @talitasa507
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
talitasa507/talitasa507 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

def calcular():
    while True:
       
        num1 = input("Digite o primeiro número: ")
        num2 = input("Digite o segundo número: ")

        try:
            num1 = float(num1) if '.' in num1 else int(num1)
            num2 = float(num2) if '.' in num2 else int(num2)
        except ValueError:
            print("Por favor, insira números válidos.")
            continue
      
        print("\nEscolha a operação:")
        print("1. Soma")
        print("2. Subtração")
        print("3. Multiplicação")
        print("4. Divisão")
        print("5. Sair")

            operacao = input("\nDigite o número da operação desejada: ")
      
        if operacao == '1':
            print(f"\nResultado: {num1} + {num2} = {num1 + num2}\n")
        elif operacao == '2':
            print(f"\nResultado: {num1} - {num2} = {num1 - num2}\n")
        elif operacao == '3':
            print(f"\nResultado: {num1} * {num2} = {num1 * num2}\n")
        elif operacao == '4':
            if num2 != 0:
                print(f"\nResultado: {num1} / {num2} = {num1 / num2}\n")
            else:
                print("\nErro: Divisão por zero não é permitida.\n")
        elif operacao == '5':
            print("\nSaindo da calculadora. Até mais!")
            break
        else:
            print("\nOpção inválida. Tente novamente.\n")


calcular()
