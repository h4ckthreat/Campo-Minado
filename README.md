# <i> Campo Minado. </i> 🕹️
# <i> Jogo campo minado com níveis de dificuldade. </i> 🕹️

O jogo Campo Minado é um jogo de tabuleiro em que o jogador deve desvendar células em um campo minado sem acertar uma mina. Cada célula pode estar vazia ou conter uma mina. Ao selecionar uma célula vazia, o jogo revela o número de minas nas células vizinhas. Com base nessas informações, o jogador deve deduzir a localização das minas e evitar revelar uma célula com uma mina.

O objetivo do jogo é revelar todas as células vazias sem acertar uma mina. Se o jogador revelar uma célula com uma mina, o jogo termina e o jogador perde. Se todas as células vazias forem reveladas, o jogador vence.

Durante o jogo, o jogador pode marcar células suspeitas de conterem minas para ajudar na dedução. Marcadores são usados para indicar essas células. No entanto, os marcadores não têm efeito direto no jogo e servem apenas como uma ajuda visual.

O tamanho do campo minado e o número de minas podem variar, e a dificuldade do jogo aumenta à medida que o tamanho do campo e o número de minas aumentam.

O Campo Minado é um jogo de lógica e estratégia que requer pensamento analítico e dedutivo para evitar as minas e revelar as células corretas.

O programa utiliza várias funções de uma biblioteca personalizada chamada "conio", incluindo manipulação de cor do texto e limpeza da tela do console.

Aqui está uma explicação da estrutura e funcionalidade do programa:

1. Os arquivos de cabeçalho necessários são incluídos: `conio.c`, `time.h`, `locale.h` e `conio.h`.
2. A função `main()` é definida.
3. O programa apresenta um menu com três opções: iniciar o jogo, opções do jogo ou sair do jogo.
4. A entrada do usuário é obtida para selecionar uma opção, e é realizada uma validação da entrada para garantir uma escolha válida.
5. O programa usa uma declaração switch para lidar com a opção selecionada:
   - Opção 1: Inicia o jogo Campo Minado.
   - Opção 2: Exibe as opções do jogo (nível de dificuldade).
   - Opção 3: Sai do jogo.
6. A lógica do jogo Campo Minado é implementada dentro do primeiro caso (opção 1) da declaração switch.
   - O jogo inicializa um array `campo` para armazenar o campo minado, juntamente com outras variáveis necessárias.
   - Números aleatórios são gerados para determinar a posição das minas e inicializar o campo minado.
   - O loop principal do jogo começa com a etiqueta `monta_tela` e exibe o tabuleiro do jogo, número de bombas e movimentos restantes.
   - O usuário seleciona uma posição no tabuleiro e a revela.
   - Dependendo da posição selecionada, células vizinhas são reveladas recursivamente até que todas as células apropriadas sejam descobertas.
   - Se a posição selecionada contiver uma mina, o jogo termina e todas as minas são reveladas.
   - Se o tabuleiro do jogo for completamente revelado sem atingir uma mina, o jogador vence.
7. O programa fornece alguns feedbacks visuais básicos usando cores de texto para representar diferentes elementos do jogo.
