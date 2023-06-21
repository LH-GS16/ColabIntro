# ColabIntro
Colab para disciplina de introdução
O código descrito cria uma rede neural convolucional para classificação de imagens usando o conjunto de dados CIFAR-10. Explicando detalhadamenta cada passo que ele faz
  1.  Carrega o conjunto de dados CIFAR-10, que consiste em imagens de 10 classes diferentes (por exemplo, aviões, carros, pássaros, gatos, etc.):
  2.  Normaliza os valores dos pixels das imagens para que estejam entre 0 e 1:
  3.  Define uma lista com os nomes das classes:
  4.  Plota uma grade de 25 imagens de treinamento com seus rótulos correspondentes:
  5.  Cria um modelo de rede neural sequencial:
  6.  Adiciona uma camada de convolução com 32 filtros de tamanho 3x3 e função de ativação ReLU, com uma forma de entrada de (32, 32, 3) (altura, largura,         canais   de cor)
  7.  Adiciona uma camada de max pooling com um fator de subamostragem de 2x2:
  8.  Adiciona outra camada de convolução com 64 filtros de tamanho 3x3 e função de ativação ReLU:
  9.  Adiciona outra camada de max pooling com um fator de subamostragem de 2x2:
  10.  Adiciona uma terceira camada de convolução com 64 filtros de tamanho 3x3 e função de ativação ReLU:
  11.  Imprime um resumo do modelo, mostrando as camadas e o número de parâmetros:
  12.  Adiciona uma camada Flatten para converter os mapas de características em um vetor unidimensional:
  13.  Adiciona uma camada Dense (totalmente conectada) com 64 neurônios e função de ativação ReLU:
  14.  Adiciona uma camada Dense (totalmente conectada) com 10 neurônios (correspondendo às 10 classes do conjunto de dados CIFAR-10):
  15.  Compila o modelo, especificando o otimizador, a função de perda e as métricas a serem utilizadas durante o treinamento:
  16.  Treina o modelo utilizando os dados de treinamento e valida-o usando os dados de teste, durante 10 épocas:
  17.  Plota a acurácia do treinamento e da validação ao longo das épocas:
  18.  Avalia o modelo nos dados de teste, calculando a perda e a acurácia:
  19.  Plota uma imagem de teste específica e exibe o rótulo predito pelo modelo:
Este código cria, treina e avalia uma CNN para classificar imagens do conjunto de dados CIFAR-10, e também exibe a predição do modelo para uma imagem de teste específica.
