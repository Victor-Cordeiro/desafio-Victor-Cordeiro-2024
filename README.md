Desafio técnico START DB
O DESAFIO
Olá! Você foi contratado para ajudar na organização de um zoológico. Sua missão será construir a lógica para indicar os recintos onde novos animais se sintam confortáveis.
RECINTOS EXISTENTES
![image](https://github.com/user-attachments/assets/5d780e84-60e8-4760-911f-6ed99e4d3616)

![image](https://github.com/user-attachments/assets/29dcc102-36a0-471f-a2f1-f3f366b44798)


**REGRAS PARA ENCONTRAR UM RECINTO**
Um animal se sente confortável se está num bioma adequado e com espaço suficiente para cada indivíduo

Animais carnívoros devem habitar somente com a própria espécie

Animais já presentes no recinto devem continuar confortáveis com a inclusão do(s) novo(s)

Hipopótamo(s) só tolera(m) outras espécies estando num recinto com savana e rio

Um macaco não se sente confortável sem outro animal no recinto, seja da mesma ou outra espécie

Quando há mais de uma espécie no mesmo recinto, é preciso considerar 1 espaço extra ocupado

Não é possível separar os lotes de animais nem trocar os animais que já existem de recinto (eles são muito apegados!). Por exemplo, se chegar um lote de 12 macacos, não é possível colocar 6 em 2 recintos.

**ENTRADAS E SAÍDAS**

O programa deve receber tipo e quantidade de animal (nessa ordem)

O programa deve retornar uma estrutura contendo a lista de todos os recintos viáveis ordenada pelo número do recinto (caso existam) e a mensagem de erro (caso exista)

A lista de recintos viáveis deve indicar o espaço livre que restaria após a inclusão do(s) animal(is) e o espaço total, no formato "Recinto nro (espaço livre: valorlivre total: valortotal)"

Caso animal informado seja inválido, apresentar erro "Animal inválido"

Caso quantidade informada seja inválida, apresentar erro "Quantidade inválida"

Caso não haja recinto possível, apresentar erro "Não há recinto viável"


EXEMPLOS
Entrada para um caso válido
"MACACO", 2

Saída
{
  recintosViaveis: ["Recinto 1 (espaço livre: 5 total: 10)", 
   "Recinto 2 (espaço livre: 3 total: 5)", 
   "Recinto 3 (espaço livre: 2 total: 7)"]
}

Entrada para um caso inválido
"UNICORNIO", 1

Saída
{
  erro: "Animal inválido"
}

