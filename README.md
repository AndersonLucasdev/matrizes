# matrizes
matrizes em python
## matriz
lista = []
linhas = int(input("Digite quantas linhas tem: "))
colunas = int(input("Digite quantas colunas tem: "))
contador = 0
lista2 = []
while contador < linhas:
    contador2 = 0
    lista2 = []
    while contador2 < colunas:
        item_linha = int(input("Digite os itens da matriz: "))
        aux = lista2
        aux.append(item_linha)
        contador2 += 1
    lista.append(aux)
    contador += 1
for x in lista:
    print(x)
print("matriz")

## matriz transposta
contador = 0
coluna = []
coluna2 = []
while contador < colunas:
    contador2 = 0
    aux = []
    coluna2 = []
    while contador2 < linhas:
        aux = coluna2
        aux.append(lista[contador2][contador])
        contador2 += 1
    coluna.append(aux)
    contador += 1
for y in coluna:
    print(y)
print('matriz transposta')
