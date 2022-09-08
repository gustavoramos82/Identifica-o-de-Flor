# Identificação de Flores

Neste projeto, a partir de um dataset obtido no kaggle (que pode ser acessado [aqui](https://www.kaggle.com/datasets/nadyana/flowers)) no qual o dataset nos fronece cinco tipo de flores para classificar, mas pelo melhor processamento foi escolhido apenas três neste projeto, que foram: Bellflower, Daisy e Dandellion.

Será utilizado uma rede neural já treinada como base e a partir disso utilizar extração de caracteristicas e fine-tunning.

Podemos ver que cada um classificador tem 1600 imagens, vendo que o mesmo está balanceado em questão das labels:

![image](https://user-images.githubusercontent.com/39843884/189103451-c22d28f3-7a5e-4c9a-83ea-454dbd71cc69.png)

## Extração de Caracteristicas

Como rede neural de base, tanto para extração de caracteristicas, quanto para fine-tunning foi utilizada foi o *InceptionResNetV2* no qual, na extração de caracteristicas teve os sguintes resultado com a tabela abaixo:

![image](https://user-images.githubusercontent.com/39843884/189104123-bfa37c8b-a5a5-4c50-b9a3-0f05963060ed.png)

Podemos ver que os modelos que teve a melhores perfomace foi o SVM e o Ridge Classifier.

## Fine Tunning

Aplicando o fine tunning tivemos o seguinte resultado:

![image](https://user-images.githubusercontent.com/39843884/189105202-75dc571d-e094-4a87-9e6a-01846d3db9a0.png)

## Conclusão

Podemos ver que o fine tunning teve um bom resultado, mas não melhor que os dois apontados na extração de caracteristicas, observa-se a limitação deste projeto por parte de hardware e não pode se ver como teste outros modelos e verificar quanto aos cinco tipos, algo que pode ser testado no futuro.
