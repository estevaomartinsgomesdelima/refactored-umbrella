from random import randint
from time import sleep
computador = randint(0 , 5) #Faz o computador pensar
print('\033[34m-=-' *20)
print('\033[35mVou pensar em um número entre 0 a 5. Tente advinhar...')
print('\033[34m-=-' *20)
jogador = int(input('\033[33mEm que número que eu pensei?'))#Jogador tente adivinhar
print('\033[35mPROCESSANDO...')
sleep(3)
if jogador == computador:
    print('\033[32mPRABÉNS! Você me venceu.')
else:
    print('\033[31mEu ganhei!Eu pensei no número {} eu não pensei no número {}.'.format(computador, jogador))
