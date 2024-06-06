# Primeiro Erro
Código feito para tratamento de erros no projeto

# Exemplo de código para tratamento de erros em Python
    try:
      a = int(input('Digite um numerador: '))
      b = int(input('Digite um denominador: '))
      res = a / b
      
    except ZeroDivisionError:
      print('Não é possivel dividir por zero!')
    except KeyboardInterrupt:
      print('O usuario preferiu não informar os dados')
    except ValueError:
      print('Digite um número inteiro!')
    except Exception as erro:
      print(f'Ocorreu o erro {erro.__class__}')
    else:
      print(f'O resultado é de {a}/{b} é {res}') 
    finally:
      print('A prática leva a perfeição')
