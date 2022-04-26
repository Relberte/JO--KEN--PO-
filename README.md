# JO--KEN--PO-
jogo de pedra, papel, tesoura em python
from random import randint
itens = ('pedra','papel','tesoura')
computador = randint(0 , 2)
print('''suas opções : 
[ 0 ] PEDRA
[ 1 ] PAPEL
[ 2 ] TESOURA''')
jogador = int(input('faça sua jogada : '))
print('-='*11)
print('jogador jogou {}'.format(itens[jogador]))
print('computador jogou {}'.format(itens[computador]))
print('-='*11)
if computador == 0:
    if jogador == 0:
        print('EMPATE')
    elif jogador == 1:
        print('JOGADOR VENCE')
    elif jogador == 2:
        print('COMPUTADOR VENCE')
    else:
        print('jogada invalida, TENTE NOVAMENTE.')
elif computador == 1:
    if jogador == 0:
        print('COMPUTADOR VENCE')
    elif jogador == 1:
        print('EMPATE')
    elif jogador == 2:
        print('JOGADOR VENCEU')
    else:
        print('jogada invalida')
elif computador == 2:
    if jogador == 0:
        print('JOGADOR VENCEU')
    elif jogador == 1:
        print('COMPUTADOR VENCEU')
    elif jogador == 2:
        print('EMPATE')
    else:
        print('jogada invalida, TENTE NOVAMENTE.')
