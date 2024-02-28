# Processamento de Linguagem Natural com Azure.

---

## Language Studio 

### Análise de texto e resposta a perguntas
Seu proposito é ter um conjunto de ferramentas baseadas no cenário de interface do usuário que vai permitir criar, integrar e explorar recursos de linguagem através de uma plataforma que nos traz ideias sobre o assunto que esta sendo escrito. 

Dessa forma, partir de uma mensagem ele vai conseguir extrair informações, como: o idioma, o sentimento, a palavra/frase chave, localidade entre outras informações conforme a frase. Assim a ferramento consegue compreender o idioma e classificar de forma personalizada a informação. Assim, é possível criar um recurso com diversos cenários para metrificar as informações apresentadas. Como, por exemplo, o quão felizes estão e qual a localidade.
Com base nessas informações é possível inserir perguntas e respostas, inserir um documento com perguntas frequentes e ser usado em bate-papos como bot chat. 

### Serviço de bot do Azure
O serviço utiliza a linguagem de IA do Azure como o próprio serviço de bot do Azure, sendo necessário inúmeras informações, o que irá medir o quão eficiente será o serviço. 

### Compreensão da Linguagem Coloquial 
A compreensão da linguagem coloquial, linguagem do dia a dia como ocorre com a Alexa quando é pedido algo. Esse modelo é formado por 3 componentes, sendo: a declaração do que pode ser dito, o que preciso que a IA faça; A entidade é um item especifico como uma automação e reconhecimentos de itens como a TV; intensão identifica a intensão do usuário em fazer algo. 
A ideia é que possa dar ordens para o dispositivo com uma linguagem do dia a dia. 
O reconhecimento e síntese da fala trabalha em um cenário de bot/conversa, mas de forma que a fala do serviço Fala fique de forma audível, utilizando um serviço de conversão de texto para fala, assim como a conversão da fala em texto.

Acesso o [Speech Studio](speech.microsoft.com/portal) .

---
### Passo a Passo da Atividade

Com o acesso ao Speech Studio, iremos em configurações criar um novo recurso. 

![download](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/df0adc39-e6ee-4151-a698-9ce900f47fab)

Após o cadastro recurso, selecione e clique para utilizá-lo.

Voltando a página inicial iremos em "Conversão de fala em texto em tempo real" e escolheremos um áudio para testar o serviço. 

![download (1)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/68ad651c-cc60-4bb2-bfe3-6c701024c0e7)

Após a verificação do serviço do Speech Studio, iremos verificar o serviço do Language Studio, que vai ajudar a fazer uma análise semântica do texto (análise de sentimentos), irá interpretar o texto. 

No Microsoft Azure, iremos criar um novo recurso com o Language service. 

![download (2)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/a94e89c5-2012-4765-a057-0fbae6fb95df)

Mantenha todas as features e clique para continuar e criar. 

![download (3)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/4f040d6c-3f98-4ba5-993f-16f8458dee6b)

Será apresentado a tela padrão de criação de recursos do Microsoft Azure. In Pricing tier selecione o F0. Então clique em "Reviwer + Create" para validar e depois em Create.

![download (4)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/c40027bc-d4df-4c32-8a26-e3365c17c92b)

Após a finalização da validação e criação, iremos para a página do language cognitive (language.cognitive.azure.com). Faça o login para o sistema identificar o recurso criado na etapa anterior. Preencha o que for necessário e clique em Done.


Eremos em Classificação de Texto  e depois em Analisar Sentimentos e Opiniões.  Selecione o idioma e informe o texto ou arquivo de texto para examinar. 

Após realizar os testes, exclua os recurso criados. 