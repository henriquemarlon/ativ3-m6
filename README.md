# Processamento de imagens e detecção de objetos

Para realizar essa atividade, foram empregadas duas fases distintas: o treinamento do modelo utilizando a versão 8 do YOLO (You Only Look Once) e a implementação em tempo real do modelo, fazendo uso da câmera do notebook.

No primeiro estágio, foi utilizado o ambiente do Google Colaboratory para executar o treinamento do modelo. Nesse processo, empregou-se um conjunto de dados específico para treinar o modelo de detecção de rachaduras, fornecido pelo Roboflow. Após a importação e preparação desse conjunto de dados, o treinamento do modelo foi conduzido ao longo de 10 épocas. Ao término desse treinamento, é possível obter um arquivo com a extensão ".pt", que representa o modelo treinado. Tal arquivo armazena os parâmetros adquiridos durante o processo de treinamento, incluindo pesos e configurações específicas do modelo.

Na segunda fase, o arquivo ".pt" foi utilizado para aplicar o modelo treinado e efetuar a detecção em tempo real de rachaduras, utilizando a câmera integrada ao notebook. Com esse propósito, um script em Python foi desenvolvido, o qual permite acessar a câmera do notebook e submeter os quadros capturados à detecção do modelo. Ao processar cada frame obtido pela câmera, o modelo treinado é capaz de identificar a presença de rachaduras e, caso detecte alguma, demarca a região correspondente desenhando um retângulo ao redor da mesma.
 
 Video: https://drive.google.com/file/d/1Azm9uZ-otGJPdJZaab5iYAsOXD-JIfz0/view
