# Imarket
MercadoNegro




# -*- coding: utf-8 -*-

print('Bem-vindo ao Imarket!')
listaMenu = []


def exibirMenu():
    # Pagina inical
    print('1-Acessar')
    print('2-Cadastrar')
    print('3-Sair')
    opt = int(input('Escolha uma opção:'))
    return opt
    listaMenu.append([opt])


#exibirMenu()
listaCliente = []


def cadastrarCliente():
    # Realiza cadastro do cliente
    nomeCliente = str(input('Nome:'))
    telefoneCliente = str(input('Telefone:'))
    emailCliente = str(input('Email:'))
    verifc = int(input('1-Comprador 2-vendedor :'))
    if verifc == 1:
        rg = int(input('RG:'))
        # RG sera o id do cliente
    elif verifc == 2:
        cnpj = int(input('CNPJ:'))

    # CNPJ sera o id da empresa
    enderecoCliente = str(input('Endereço:'))
    senhaCliente = str(input('Digite sua senha:'))
    confirmSenha = str(input('Repita a senha:'))

    if senhaCliente == confirmSenha:
        print('Cadastro concluído!')

    else:
          print('Senhas não compativeis')
          print('Tente oura senha')
          print('Cadastro cancelado')
          listaCliente.append([nomeCliente, telefoneCliente, emailCliente, rg, cnpj, enderecoCliente])


# chama lista de funçoes para cadastrar clientes
#cadastrarCliente()

listaCadastro = []


def acessarCadastro():
    cadastrarCliente(rg, cnpj, senhaCliente)
    # chama o id do cliente e senha

    login = int(input('RG/CNPJ:'))
    if login == rg:
        password = int(input('Senha:'))
        if password == senhaCliente:
            print('Acesso confirmado')
    elif login == cnpj:
        password = int(input('Senha:'))
        if password == senhaCliente:
            print('Acesso confirmado')
            def opcoes():
                print('1-Cadastrar produto:')
                print('2-modificar preço:')
                print('3-sair:')
                esc= int(input('entre com uma opção:'))
             nomeprodt=[]
             codprodt=[]
             valorprodt=[]
             validadeprodt=[]
             listaprodt[nomeprodt, codprodt, valorprodt, validadeprodt]
            nomeprodt = 0
            codprodt = 0
            valorprodt = 0
            validadeprodt = 0

            def cadastrar_Produto(prodt=None):
                codprodt=int(input('Cod do produto:'))
                nomeprodt=input('Nome do produto:')
                valorprodt=float(input('valor do produto:'))
                validadeprodt=input('Validade do produto:')
                listaprodt.append([codprodt, valorprodt, nomeprodt, validadeprodt])
            pass



            while True:
                if esc==1:

                elif esc==2:

                elif ssc ==3:

                    break



    listaCadastro.append([login, passaword])
#acessarCadastro()

# Aqui tava errado, tem que ler a opção antes de de testar, mas dentro do while
while True:
    opt = exibirMenu()
    if opt ==1:
        acessarCadastro()

    elif opt == 2:
        cadastrarCliente()
    else:
         print('Desconectado!')
         exit()  # Aqui chama exit para terminar o programa
    break
