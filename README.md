# Azure Cognitive Search: Utilizando AI Search para consulta de Dados

Passo a passo do desafio de projeto "Azure Cognitive Search: Utilizando AI Search para consulta de Dados" da DIO.

Links importantes:

[Explore an Azure AI Search index (UI)](https://aka.ms/ai900-ai-search)

[Zip com os reviews](https://aka.ms/mslearn-coffee-reviews)

## Passo 1: Criando recursos necessários no Portal do Azure

Primeiro precisei criar um recurso do Azure AI Search dentro do Azure AI Services. Em Escalão de preço, utilizei "Básico".

![Img](./img/img1.gif)

Depois criei o recurso de Serviços Cognitivos.

![Img](./img/img2.gif)

E após criei uma conta de armazenamento.

![Img](./img/img3.gif)

Para configurá-la com configurações básicas apenas para este laboratório, precisei liberar o acesso ao container de Blob para anônimos em Menu lateral na página do recurso > Configurações > Permitir acesso anônimo de Blob.

![Img](./img/img4.gif)

## Importando dados

Para importar os dados, acessei "Armazenamento de dados" > "Contentores" para trazer arquivos. Criei um novo container com o nome coffereview e o nível de acesso como "Contentor (Acesso a leitura anônima para contentores e blobs)".

![Img](./img/img5.gif)

Acessei o contentor que acabei de criar e cliquei no botão "Carregar". Então fiz o upload dos arquivos de texto disponíveis em https://aka.ms/mslearn-coffee-reviews.

![Img](./img/img6.gif)

Então acessei o recurso criado para o AI Search e "Importar dados".

Para importar os dados, segui o tópico "Indexar os documentos" deste artigo (https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html).

## Testando a pesquisa

Para fazer o teste, acessei a aba "Explorador de procura" da página do recurso de pesquisa.

Fiz uma pesquisa sobre localidade:

_search=locations:'Chicago'_

![Img](./img/img8.png)

E outra pesquisa sobre opiniões positivas:

_search=sentiment:'positive'_

![Img](./img/img10.png)
