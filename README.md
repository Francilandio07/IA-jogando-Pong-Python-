# IA-jogando-Pong-Python-
## Descrição
No arquivo "Game.py" está implementado o código de um jogo que consiste de dois elementos: Uma raquete e uma bola. No jogo a pontuação é incrementada sempre que a raquete impede que a bola colida com a extremidade esquerda da tela e para isso é necessário que a raquete esteja antecipadamente cobrindo o local de incidência da bola nesta área descrita. A bola inicialmente é "spawnnada" de forma aleatória na cena e começa a se mover colidindo nas extremidades da tela, de modo periódico varrendo toda a dimensão horizontal, indo e vindo.

No código desenvolvido uma rede neural simples é implementada e por reforço ela aprende a jogar o jogo visando sempre aumentar sua pontuação. Essa rede (feedforward) é composta por dois neurônios na camada de entrada, dois neurônios na única camada oculta e um neurônio na camada de saída. A aprendizagem se baseia em penalizações e recompensas de modo que o modelo é penalizado sempre que o centro da raquete está desalinhado com a bola no eixo y e também quando a bola bate na extremidade esquerda da tela, sendo esta última uma penalização de maior peso, as recompensas ocorrem em situações opostas às descritas.

A decisão da rede neural a cada iteração é de mover a raquete para cima ou para baixo de acordo com a saída, a mesma incorpora uma boa desenvoltura a partir de seus erros e atualização dos pesos de suas camadas que de início são todos aleatórios.

##Visão do Jogo rodando
<p align="center">
  <img width="600" height="400" src="https://user-images.githubusercontent.com/58220640/184260807-825cf303-0fdb-4fc7-8be2-88f2446ed550.gif">
</p>

