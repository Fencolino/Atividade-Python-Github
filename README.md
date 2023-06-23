# Atividade-Python-Github
Aluno: Lucas Rodrigues Pinheiro                    Colab para a disciplina de Introdução

No primeiro bloco tem como função declarar as bibliotecas que serão usadas nesses codigos, sendo elas a OpenCV e a Numpy. OpenCV é uma biblioteca de processamento de imagem que permite apresentar a visão computacional. Ja a biblioteca numpy é para trabalhar com computação numerica. Esse processo se repete duas vezes tanto para se utilizar no google colab quanto no proprio computador.

No segundo bloco o codigo como um todo começa declarando tres variaveis diferentes, (img, img_opening e img_closing)
isso a partir de 3 imagens disponibilizadas para nos de 3 letras j (uma com o j normal, uma com o j com furos e outra
com o j com algumas bolinhas brancas ao seu redor). Apos isso é declarado que os valores de altura e largura sera conhecido
como img.shape. E agora indo para a lado pratico da coisa, uma matriz de 5 por 5 com todas as suas casas com o valor de 1
é declarado como kernel e é então printada na tela. 

No terceiro bloco ele declara duas variaveis sendo elas erosion, sendo ligada a função cv2.erode, e a a varivel dilation, sendo ligada com uma outra função chamada cv2.dilate. Dei uma breve pesquisada para entender a respeito desses dois procedimentos de imagem, e descobri que a função erosion ira diminuir as caracteristicas de uma imagem, ja a dilation serve para aumentar as caracteristicas visuais de uma imagem, isso tudo sendo interligado com as imagens do 3 j e com a matriz 5 por 5.

No quarto bloco é declarado 3 variaveis sendo elas gradient, opening, closing. Gradient esta sendo ligado a um cv2.morphologyEx, e dentro desse seus parenteses ele se vincula com a variavel img, com cv2.MORPH_GRADIENT e com a matriz kernel. As duas proximas variaveis opening e closing ambas se igualam com um cv2.morphologyEx, de maneira respectiva (opening e closing) se interligam com as variaveis img_opening e img_closing, na proxima se vinculam com cv2.MORPH_OPEN e cv2.MORPH.CLOSE e todos terminando com a matriz 5 por 5 kernel.

No quinto e ultimo bloco é momento de saida dos dados. No caso do Python no proprio computador todas as saidas começam com cv2.imshow, tendo um comando de saida terminado em out, e logo apos isso uma ligação com as variaveis anteriormente declaradas. Dessa forma a escrita fica da seguinte forma, ('in', img) para a imagem padrão, ('erosion_out', erosion) para a função de erosion, ('dilation_out', dilation) para a função de dilation, ('opening_out', opening) para a opening da imagem, ('closing_out', closing) para o closing da imagem e ('gradient_out', gradient) para o gradient da imagem. Ja no google colab a forma de saida é mais facil começando com cv2_imshow e entre parenteses apenas a varivel, sendo elas img,erosion,dilation,opening,closing e gradient.

Link de informações: https://acervolima.com/erosao-e-dilatacao-de-imagens-usando-opencv-em-python/
                     https://medium.com/data-hackers/gradientes-descendentes-na-prática-melhor-jeito-de-entender-740ef4ff6c43

                     

