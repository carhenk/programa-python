# programa-python

#descrição: Crie um programa onde o usuario tem 3 chances de acertar a senha secreta
#encerre o loop ao acertar ou esgotar as tentativas.

senha_secreta = "2552" # Defina a Senha Secreta
tentativas = 3
while tentativas > 0:
  senha = input("Digite a Senha:")
  if senha == senha_secreta:
    print("Senha correta! Acesso Permitido.")
    break
  else:
    tentativas -= 1
    print(f"Senha incorreta! Você tem {tentativas} tentativa(s) restante(s).")
  if tentativas == 0:
    print("Todas as Tentativas esgotadas. Acesso Negado.")
    
