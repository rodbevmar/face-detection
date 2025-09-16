# Detecção de Faces com OpenCV e Google Colab

## Descrição do Projeto

Este projeto tem como objetivo realizar a detecção de faces em imagens utilizando a biblioteca OpenCV e o ambiente Google Colab. O fluxo principal envolve a captura de uma foto via webcam, processamento da imagem e identificação de faces utilizando um modelo pré-treinado baseado em Deep Learning.

## Principais Etapas

1. **Importação de Bibliotecas**  
   Utiliza-se `imutils`, `numpy`, `cv2`, além de recursos do Google Colab para captura e exibição de imagens.

2. **Captura de Imagem**  
   A imagem é capturada diretamente da webcam do usuário por meio de um script em JavaScript integrado ao Colab.

3. **Pré-processamento da Imagem**  
   A imagem capturada é redimensionada para facilitar o processamento e visualização.

4. **Download dos Pesos do Modelo**  
   Os arquivos `deploy.prototxt` e `res10_300x300_ssd_iter_140000.caffemodel` são baixados para realizar a detecção de faces.

5. **Carregamento do Modelo**  
   O modelo é carregado utilizando a função `cv2.dnn.readNetFromCaffe`.

6. **Detecção de Faces**  
   A imagem é convertida em blob e passada pelo modelo para identificar possíveis faces. As detecções com confiança acima de 50% são destacadas com caixas delimitadoras e a porcentagem de certeza.

7. **Exibição do Resultado**  
   A imagem final, com as faces detectadas, é exibida diretamente no notebook.

## Requisitos

- Python 3.x
- OpenCV
- imutils
- Google Colab

## Como Executar

1. Faça upload do notebook no Google Colab.
2. Execute as células sequencialmente.
3. Permita o acesso à webcam quando solicitado.
4. Visualize o resultado da detecção de faces na imagem capturada.

## Referências

- [Documentação OpenCV](https://opencv.org/)
- [Google Colab](https://colab.research.google.com/)
- [Modelo SSD Face Detector](https://github.com/opencv/opencv/tree/master/samples/dnn/face_detector)
