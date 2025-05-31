print("""
====================================
- interface: calcular media da unip
====================================
""")
nome = input("digite o seu nome:\n")
ra = input("digite o seu ra:\n")

print("ola tudo bem Sr.",nome,"bem-vindo ao sistema para calcular media da unip:" )

menu = print("""
==============================================

qual dessa opçoes para calcular media:

1.calcular a media da np1 np2 e o pim:

2.calcular a media do exame

3.sair do sistema

===============================================
""")
while True:
  x = input("digite a opção: ")
  if (x == "1"):
        np1 = float(input("nota np1:"))
        np2 = float(input("nota np2:"))
        pim = float(input("nota do pim:"))
        media = (4 * np1 + 4 * np2 + 2 * pim) / 10
        print(f"{media}")
        if media >= 7.0:
            print("PARABENS!! O SR ESTA APROVADO DESSA MATERIA.")
        else:
            print("INFELIZMENTE O SR FICOU DE EXAME DESSA MATERIA.")
  elif (x == "2"):
        notafinal = float(input("nota da media final:  "))
        notadoexame = float(input("nota do exame: "))
        mediae = (notafinal + notadoexame) / 2
        print(f"{mediae}")
        if mediae >= 5.0:
         print("PARABENS!! O SR CONSEGUIU PASSA DO EXAME!!")
        else:
            print("INFELIZMENTE SR FICOU DE DP")
  elif (x == "3"):
    print("VC SAIU DO SISTEMA...")
    break
