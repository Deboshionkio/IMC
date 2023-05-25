# IMC
Bloco de Código para Calcular o Índice de Massa Corporal
# Índice de Massa Corporal

# Nesta parte do código vamos receber do usuário o seu peso e altura
peso = float(input('Insira seu peso: '))
altura = float(input('Insira sua altura: '))

# Agora para o cálculo, dividindo o peso pela altura ao Quadrado
imc = peso / (altura ** 2)

# Menor que 18.5 - abaixo do peso normal; Menor que 25.0 - peso normal; Entre 25.0 e 29.9 - Pré-obesidade ;
# Entre 30.0 e 34.9 - Obesidade Grau 1 ; Entre 35.0 e 39.9 - Obesidade Grau 2 ; Acima de 40 - Obesidade Grau 3
# vamos fazer a informação do imc, conforme a tabela de pesos e seus índices

if imc < 18.5:
    print(f'Você está com o imc = {imc:.2f}, abaixo do peso!')
elif imc < 25:
    print(f'Você está com o imc = {imc:.2f}, parabéns, peso normal!')
elif imc < 30:
    print(f'Você está com o imc = {imc:.2f}, Pré Obesidade!')
elif imc < 35:
    print(f'Você está com o imc = {imc:.2f}, Obesidade Grau 1!')
elif imc < 40:
    print(f'Você está com o imc = {imc:.2f}, Obesidade Grau 2!')
else:
    print(f'Você está com o imc = {imc:.2f}, Obesidade Grau 3!')
