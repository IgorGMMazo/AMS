# Preparar o ambiente

    Usar Python 3 (de preferência 3.9+).

    Instalar as bibliotecas principais:

# Escolher uma imagem de teste

    Pode ser qualquer foto que tenha um objeto “claro”: cachorro, gato, carro, etc.

    Salve a imagem na mesma pasta do script/notebook

# Carregar o AlexNet pré-treinado

    Vamos usar torchvision.models.alexnet com pesos treinados no ImageNet.

    Isso permite mostrar inferência sem treinar nada, só aproveitando o modelo pré-treinado.

# Preparar as transformações da imagem

    O AlexNet espera imagens em um formato específico:

    Tamanho: 224x224 e 3 canais (RGB).

    Normalização usando média e desvio padrão do ImageNet.

    Vamos usar as transforms prontas que vêm junto com os pesos.

# Fazer o pré-processamento e criar o batch

    Abrir a imagem com PIL.

    Converter para RGB.

    Aplicar as transforms.

    Adicionar uma dimensão de “lote” (batch) para ficar com shape [1, 3, 224, 224].

# Rodar a inferência

    Colocar o modelo em modo de avaliação: model.eval().

    Desligar o cálculo de gradiente com torch.no_grad().

    Passar o batch pelo modelo.

# Calcular probabilidades e pegar as top-5 classes

    Aplicar softmax na saída.

    Usar torch.topk para pegar as 5 classes mais prováveis.

    Traduzir índices (0 a 999) para nomes de classes usando weights.meta["categories"].

# Mostrar o resultado