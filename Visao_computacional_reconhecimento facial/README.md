## Reconhecimento de imagem
---

Na análise de imagem 4.0 como AI Vision Service, a imagem é analisada e rotulada para identificar o que existe nessa imagem, se existe uma pessoa, se essa pessoa é mulher ou homem, qual roupa esta usando. 

Também é possível trabalhar com reconhecimento facial na Pesquisa visual computacional detectando as características e acessórios, grandemente utilizada no seguimento de segurança, identificando se essa pessoa está, por exemplo, sendo procura pela polícia.
Com o Face Service, é possível comparar os rostos e identificar a pessoa. 

No serviço de OCR, trabalhamos com a leitura de textos em uma imagem e reconhecimento óptico de caracteres. Detectando a localização do texto impresso ou escrito a mão a depender da validação e treinamento. Esse serviço pode ser utilizado na leitura de uma comprovante para salvar e classificar o tipo de comprovante, valor e demais informações deste, o que pode ser útil em empresas de transporte que precisar registrar os custos de uma viagem, por exemplo. 
Quando falamos em textos escritos a mão é importante se atentar em ser uma letra legível. 

Já a Analise espacial, quando a IA analisa a imagem e identifica o que existe nela, trazendo uma descrição da imagem pode ser usado em situações de acessibilidade permitindo que uma pessoa com deficiência visual possa "ver" uma imagem através da descrição da mesma. 

--- 
### Realizando o Laboratório 

Com o Microsoft Azure em "Create a resource", procuraremos pela categoria AI + Machine Learning e depois no serviço Azure Ai Servises para criar. 

A configuração funciona como uma ponte dos serviços de IA na nossa assinatura com o Vision Studio. 

Na primeira tela de configuração temos a Subscrição que é a identificação da sua conta e em seguida escolha o Resource Group, o grupo no qual esse recurso ficará armazenado, caso não tenha clique em Create para criar um e continuar com a configuração do serviço. 

Region seria a região onde você esta, porem esta sendo utilizado a região dos EUA devido a precificação ser mais barata. Em seguida informe o nome que desejar. 

Em Pricing tier selecione "Standard S0" e em seguida seleciona a caixa de seleção. 

Por ser um laboratório de estudo introdutório, os demais recursos não foram explorados, assim foi dado seguencia com o "Review+Create" e em seguida em Create.

![download](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/a986cdb8-b97a-47dc-a775-1f016a000e56)

Com o recurso criado, iremos no Vision Studio no link: https://portal.vision.cognitive.azure.com/

Acesse com a sua conta Azure e vá em "View all resorces"  e será apresentado o recurso criado na etapa anterior. 

![download (1)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/314c3132-bbee-4270-8ab4-a15fe4157bf7)

Caso não apareça confira se a criação do recurso foi finalizada e de um "Refresh" no Vision para verificar o seu recurso. 

Após encontrar o recurso, selecione e clique em "Select as default resource". Após deixar como defaul, no canto direito basta clicar em "X ". 

![download (2)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/e75e7a9f-7e2f-4e62-b4fa-e26c1f3fc877)

Após isso, voltaremos para a tela inicial aonde iremos em "Face" e em seguida em "Detect faces in an image". 

![download (3)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/25145d40-880a-4a64-9e4a-a28dd7fa1b47)

Selecione a flag do "Try it out" e abaixo é possível fazer alguns testes com as próprias imagens de exemplos fornecidas pela plataforma.  Para fazer o teste, eu precisei identificar o meu usuário e o recurso criado. Realize testes com a ferramenta, utilizando imagens diversas. 

Para fazer a análise de imagens com texto, iremos retornar a tela anterior e ir em "Optical character recognition" e abrir a ferramenta "Extract text from images". 
Realize o mesmo processo realizado com a identificação de faces. 

Também realizei testes com o serviço "Add captions to images" da aba de Image Analysis.

Após realizar os testes com as ferramentas, exclua seu recurso.

