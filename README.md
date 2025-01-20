# OCR com Azure Cognitive Services

## Introdução
Este tutorial ensina como usar o Azure Cognitive Services para extrair texto de imagens usando OCR (Reconhecimento Óptico de Caracteres).

## Pré-requisitos
- Conta no [Azure](https://portal.azure.com/)
- Azure AI Services criado
- Chave e endpoint do Azure AI Services
- Python instalado

## Passo a Passo

### 1. Criar um recurso no Azure
1. Acesse o [portal do Azure](https://portal.azure.com/).
2. Crie um recurso **Azure AI Services**.
3. Copie a **chave** e o **endpoint**.

### 2. Conecte seu recurso de serviço de IA do Azure ao Vision Studio
1. Em outra aba do navegador, navegue até o [Vision Studio](https://portal.vision.cognitive.azure.com)
2. Na página inicial do Vision Studio, selecione Exibir todos os recursos no título Introdução ao Vision.
3. Na página Selecionar um recurso para trabalhar, passe o cursor do mouse sobre o recurso que você criou acima na lista, marque a caixa à esquerda do nome do recurso e selecione Selecionar como recurso padrão.
4. Feche a página de configurações selecionando o “x” no canto superior direito da tela.

### 3. Extraia texto de imagens no Vision Studio
1. Em um navegador da Web, navegue até o [Vision Studio](https://portal.vision.cognitive.azure.com)
2. Na página inicial Introdução ao Vision , selecione Reconhecimento óptico de caracteres e, em seguida, o bloco Extrair texto de imagens.
3. No subtítulo Experimente , reconheça a política de uso de recursos lendo e marcando a caixa.

### 4. Enviar uma imagem para análise
1. No portal, selecione Browse for a file e navegue até a pasta no seu computador onde está o arquivo, selecione e click em Open.

### 5. Exibir o texto extraído
1. Agora revise o que é retornado:
    - Em Atributos detectados , qualquer texto encontrado na imagem é organizado em uma estrutura hierárquica de regiões, linhas e palavras.
    - Na imagem, a localização do texto é indicada por uma caixa delimitadora


## Referência
[Microsoft Learn - OCR com Azure Cognitive Services](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html)
