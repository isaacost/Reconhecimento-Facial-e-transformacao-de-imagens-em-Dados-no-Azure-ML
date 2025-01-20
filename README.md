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

### 2. Instalar dependências
```bash
pip install azure-ai-formrecognizer
```

### 3. Configurar credenciais
```python
from azure.core.credentials import AzureKeyCredential
from azure.ai.formrecognizer import DocumentAnalysisClient

endpoint = "SEU_ENDPOINT"
key = "SUA_CHAVE"
client = DocumentAnalysisClient(endpoint, AzureKeyCredential(key))
```

### 4. Enviar uma imagem para análise
```python
with open("imagem.jpg", "rb") as image:
    poller = client.begin_analyze_document("prebuilt-read", image)
    result = poller.result()
```

### 5. Exibir o texto extraído
```python
for page in result.pages:
    for line in page.lines:
        print(line.content)
```

## Conclusão
Agora você pode usar OCR para extrair texto de imagens com o Azure Cognitive Services!

## Referência
[Microsoft Learn - OCR com Azure Cognitive Services](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html)
