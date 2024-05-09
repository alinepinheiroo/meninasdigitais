# meninasdigitais
import math
from types import BuiltinMethodType
nome = [input('Bem vindos(as) à venda de ingressos do evento mais esperado do ano!\nInsira seu nome completo: ')]
gênero=int(input("Qual seu gênero?\n1-para feminino\n2-para masculino\n3-para outros\nDigite aqui: "))
idade=int(input("Insira sua idade: "))
email=str(input("Insira seu email: "))
pagar=int(input('Qual séra a forma de pagamento? digite:\n 1-cartão de crédito\n 2- cartão de débito\n 3- pix\n'))
if pagar==1:
  din= "cartão de crédito"
elif pagar==2:
  din= "cartão de débito"
elif pagar==3:
  din="pix"
x=60
if gênero==1 and idade<18:
   print('Olá!',(nome),'seu ingresso custará R$', (x/2),'e seu pagamento séra efetuado através do',(din),'. Enviamos para o seu email:',(email), ',todas  as informações completas do evento juntamente com o tickte de acesso à ala exclusiva para mulheres! onde séra realizado o breakcoffe com as maiores figuras femininas da tecnologia presentes na palestra.Aproveite!')
elif gênero==1 and idade>18:
   print('Olá,',(nome),'seu ingresso custará R$',(x),'e seu pagamento séra efetuado através do', (din),'. Enviamos para o seu email:',(email), ', as informações completas do evento juntamente com o tickte de acesso à ala exclusiva para mulheres! onde séra realizado o breakcoffe com as maiores figuras femininas da tecnologia presentes na palestra.Aproveite!')
elif gênero==2 or 3 and idade<18:
   print('Olá,',(nome),'seu ingresso custará R$',(x/2),'e seu pagamento séra efetuado através do', (din),'Enviamos para o seu email:',(email),', as informações completas do evento.Aproveite!')
else:
  print('Olá,',(nome),'seu ingresso custará R$',(x),'e seu pagamento séra efetuado através do', (din),'Enviamos para o seu email:',(email),', as informações completas do evento.Aproveite!')

#mudar=[input("Confere as informações acima ?\n 1-sim\n 2-não: \n")]
#nome[0]= mudar
#print(mudar)
#nome[0]= novonome
#print("seu nome foi alterado para:",nome)
#print("Certo",nome,"sua compra foi finalizada com sucesso!")
check=int(input('Confere as informações acima ?\n 1-sim\n 2-não\n:'))
if check== 1:
  print("Certo",nome,"sua compra foi finalizada com sucesso!")
else :
  novo = input("Qual dado voce deseja alterar?\n 1-nome\n 2-email\n 3-forma de pagamento\n=> ")
  if novo == '1': 
      novonome = input("Digite o novo nome: ")
      nome = novonome
      print("O nome foi alterado para:", nome)
  elif novo == '2':
      novoemail = input("Digite o novo email: ")
      email = novoemail
      print("O email foi alterado para:", email)
  elif novo == '3':
      novopagamento = input("Digite a nova forma de pagamento: ")
      pagar = novopagamento
      print("A forma de pagamento foi alterada para:", pagar)
print("Sua compra foi realizada com sucesso! ")
for c in range(1,3):
  print('FIM!!!')
    



