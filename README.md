import os
clear = lambda: os.system('cls')
clear()

print( 'Cadastro de usuário' )
print('===================')


nome = input('Informe o seu nome [minimo 4 caracteres]:')
idade = int(input('informe sua idade: '))
genero = input('Informe o gênero: ')
ano = int(input('Informe seu ano de nascimento: '))

while len(nome) <= 3:
    nome = input("Seu nome deve ter mais que 3 caracteres: ")

while (idade < 0) or (idade > 150):
    idade = int(input("Voce deve ter entre 0 e 150 anos: "))

while (genero != 'f') and (genero != 'm'):
        genero = input("Biologicamente, você deve ser 'f' ou 'm': ")
        print('genero válido')
        print(genero)

while (ano < 1900) or (ano > 2022):
            ano = int(input("Voce tem ter nascido entre 1900 e 2022: "))



subtração = int(2022) - int(ano)

while (int)(idade) != subtração:
    ano = input("data de nascimento incorreta informe a data de nascimento correta: ")
    subtração = int(2022) - int(ano)

print('Cadastro finalizado')
print('===================')
print("Nome: ", nome)
print("Gênero: ", genero)
print("Idade: ", idade)
print("Ano: ", ano)
