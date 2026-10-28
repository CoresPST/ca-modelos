# como fui trazendo os modelos pro jogo

essa parte deu trabalho kkkkk. não foi só pegar um modelo, mudar o nome do arquivo e jogar na pasta.

primeiro fui olhando os pacotes do jogo pra achar o modelo e o que vinha junto dele. usei ferramentas pra ler VPK e visualizar ou exportar recursos, tipo o Source 2 Viewer nos arquivos de Source 2.

modelo sozinho não resolve muita coisa. precisava conferir as texturas, os materiais, o esqueleto e as animações. as vezes o arquivo abria, mas dentro do jogo a mão ficava torta, a arma ficava preta ou a animação não encaixava.

ai vinha a adaptação pro formato que a nossa base usa. material de uma engine não vira material de outra automaticamente. fui ajustando a geometria e os materiais, preparando a compilação e conferindo o resultado no jogo.

tbm tem diferença entre a arma que aparece na mão e a arma que os outros jogadores veem ou que fica no chão. precisei tratar essas apresentações e os pontos onde entram os efeitos, pra não ficar tudo fora do lugar.

fui usando scripts em Python pra repetir essas etapas em vários itens e guardar os resultados. ajuda bastante pq fazer tudo na mão, um por um, vira uma bagunça rapidinho.

meu fluxo ficou tipo: achar os arquivos, extrair, conferir o que falta, adaptar, compilar e abrir no jogo pra ver. quando quebrava alguma coisa, voltava na etapa que precisava.

não modelei esses assets todos do zero. os modelos e as ferramentas usadas continuam sendo dos respectivos criadores; aqui é só um relato da parte de extração e adaptação que fiz no projeto.

[a parte do launcher ficou nesse outro repo](https://github.com/CoresPST/ca-launcher).
