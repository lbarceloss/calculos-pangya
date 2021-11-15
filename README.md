# Distancia
Vamos entender como é feito o calculo da Distancia no PangYa, Primeiro devemos saber o que é a distancia dentro do Pangya? - E simples é a diferença entre a BOLA e o HOLE!
- Tabom Leozão isso ai qualquer um sabe! Calma idiota deixa eu falar.
A Bola e o hole são objetos posicionados tridimensionalmente no MAPA o que isso significa? Significa varias coisas o interesante saber que ele possuem um (X,Y,Z).
- Tabom Leozão mais idai? O FDP eu ja falei deixa eu falar.
Segundo a formula matematica o calculo da distancia entre 2 pontos se dá pela seguinte formula:

![image](https://user-images.githubusercontent.com/82356894/141707863-b25b5a69-8fce-42c0-ac7a-bd8c7cd46b5a.png)

Então se nos temos o (X,Y,Z) do Hole e da Bola é facil calcular a distancia não é mesmo?

- Leozão seu troxa e o eixo Z?, eu fiz e deu errado, tu é burro? Caralho mano voce nao entende mesmo né deixa eu acabar de explicar depois voce pergunta.

O Eixo Y no caso seria para calcular a Altura do hole utilizando basicamente a mesma formula acima, só com o "Delta X", não deu certo ai porque voce não multiplicou a Distancia por 0.3125

Mas porque multiplicar a distancia por 0.3125? Tu nao fica me enterropendo o tempo todo Resolver ae agora o FODÃO!

# Power Bar
Vamos entender como é feito o Calculo do Power Bar no Pangya, Primeiro vamos precisar pegar o Angulo da Camera em relação a Bola e o Hole.

![image](https://user-images.githubusercontent.com/82356894/141709460-47943b12-1d82-4af7-b24d-f94d2c34e9c6.png)

- ATAN2? Cara você ta foda hoje, nada mais nada menos jovem mancebo que o angulo entre -π e π

Agora precisamos do Grid da Mira do Personagem
- Pera o que é Grid, o que é mira o que é Personagem? Calma isso merece um video de 10 minutinhos explicando tudo isso.

Com isso em maõs fica facil calcular o PB temos todo o necessario para tal.

![image](https://user-images.githubusercontent.com/82356894/141711818-9fd306d1-a90c-45ae-b8bb-74ab9e7cac99.png)
- ABS? Valor Absoluto amigo basciamente seria multiplicar um numero * -1 sempre ele for negativo no caso vou ter o retorno do numero sempre positivo exemplo -2 vira 2 -4 vira 4.
- %? Mod Amigo basicamente vai retornar o Resta da divisão, arredondando para direção retrograda no caso para 0.

Então:

![image](https://user-images.githubusercontent.com/82356894/141710816-bc3f2568-4ea8-49c1-8ad9-450a39d5e3dd.png)

- Porque dividir por 1,5 e depois 0,21657? 0,21657 e o valor de PB no PangYa e 1,5 se voce mexe com calc excel sabe muito bem que isso é a escala de Yards do Pangya.

# Quebra Bola
