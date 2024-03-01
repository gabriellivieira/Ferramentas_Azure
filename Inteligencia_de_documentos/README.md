# Inteligência de Documentos

## Mineração de conhecimento

Mineração de conhecimento é utilizado para organizar os conteúdos de uma empresa, como, por exemplo, os arquivos de uma biblioteca, agencia bancaria, um órgão governamental no qual possuem uma abundância de dados no qual podem sofrer com erros humanos e catástrofes que resultaram de perda dos dados temporários ou permanentes. 

A mineração de conhecimento é importante, pois muito do conhecimento hoje ainda se encontram em formatos físicos, no qual as empresas podem se beneficiar por meio da migração, uma vez que insights podem ser retirados por meio de palavras-chave. 

O Azure Cognitive Search é a plataforma de mineração de conhecimento alimentada pela Ia do Azure. Essa irá auxiliar na pesquisa e mineração desses dados. 

Para ingestão de dados podemos utilizar as seguintes aplicações:
* Azure Blob Storage contairners: Reconhece qualquer tipo de documento no qual pode ser apontado para uma aplicação.
* Azure Data Lake Storage Gen2: como repositório de dados. 
* Azure Table Storage: Trabalhar com tabelas. 

## Pesqusa cognitiva

Com a Pesquisa cognitiva, é possível enriquecer os índices para permitir a compreensão mais profunda dos dados, ele permite que todo o conteúdo seja pesquisável.  Esse enriquecimento acontece mediante habilidades cognitivas como visão, processamento de linguagem natural, entre outros. 

Os arquivos usados para a pesquisa deve estar em formato .json .

No tema enriquecimento de dados, falamos em trazer mais dados para garantir que a pesquisa seja mais efetiva, assim o grande volume de conteúdo permitira que os insights sejam mais assertivos. Para trazer essas informações é necessário ter acesso a esses dados, podendo ser em formato de texto, imagens, vídeos, redes sociais e também utilizar a análise de sentimentos. 

---

### Passo a Passo da Atividade
O problema a ser resolvido:
Uma rede de cafe gostaria de fazer uma pesquisa sobre a qualidade dos seus serviços. 

AISearch será usado em uma atividade de pesquisa da qualidade do serviço de uma rede, assim será verificado quais recursos serão criados, como os dados serão extraídos, como enriquecer a IA, como trabalhar com os índices e como consultar as pesquisas. 

Com acesso ao Azure, iremos pesquisar pelo Azure AI Search indo no menu da esquerda em "Create a resorce". 

![download](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/171a3509-982b-4eed-9d81-c6b2232a790e)


Clique para criar o recurso e preencha os dados solicitados, em Pricing Tier selecione a opção "Basic". 

![download (1)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/616a2976-4158-4f54-a769-4dd3d0a3cf5e)


Com o AISearch configuradora, será necessário criar um recurso de serviço IA.

![download (2)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/83018063-1959-4681-b0d0-ecb979e0f122)

![download (3)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/0ff4401b-802f-4667-9f93-f6fbb727f3c8)


Após a criação dos dois serviços, deve-se criar uma conta de armazenamento. Para isso volte para o home e clique em Storage Accounts e em criar. A configuração inicial segue o padrão dos demais serviços com o detalhe que o nome deve ser 100% único e o campo Redundancy selecione a primeira opção LRS que é um modelo de réplica dos dados que serão incluídos no Storage Account.

![download (4)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/674bb5c5-7527-4ca3-ad27-2dd999317962)


Após isso Review e Create. Com o processo finalizado faça o acesso indo em "Go recourse". 

![download (5)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/7f763b5e-bd80-44f5-83ac-633f1ca93e5f)


O storage account possui algumas regras de segurança e para realizar a atividade algumas dessas regras foram criadas para o sucesso nos testes.  Para isso, vá nas opções a esquerda, configurações e habilita a opção: "Allow Blob anonymous access" e salve.

O próximo passo é levar alguns arquivos para o container, então dentro da opção de Containers clique para criar um novo. Informe um nome e o nível de acesso como "Container".

O próximo passo é alimentar o container. É possível encontrar os arquivos na [Documentação Oficial](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html) e faça o upload dos mesmos. 

![download (6)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/55f4546b-a8c1-416f-b068-55b3583b4adc)


Agora, temos um mecanismo de busca, um serviço de IA e um repositório com informações. O próximo passo é voltar para a ferramenta de IA Search e clicar em Importar Dados e iniciar a configuração, conforme documentação do capitulo "Index the documents"

![download (8)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/08904ecd-dd7e-4ea0-ba80-54e0591a6cff)


Com os links configurados entre o Storage account com os dados e o serviço de AI Search, iremos no recurso de pesquisa e em seguida em Search explorer. 

![download (7)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/54e938b5-f57e-497b-9536-8f50d974a957)


Podemos pesquisar, por exemplo:  search=location:'Chicago' para pesquisar o que os clientes estão dizendo sobre os cafés nessa localidade.

A documentação possui outros códigos .json que podem ser testados. 

Foi criado um serviço de IA com a automação e a partir disso foi direcionado para um repositório. Assim, com os dados salvos foi possível fazer uma busca pela Search utilizando a automação, mas também é possível utilizar o serviço em uma aplicação. 

Após finalizar exclua todos os recursos criados. Uma forma simples de fazer isso é excluir o grupo com todos os recursos inclusos. 
 