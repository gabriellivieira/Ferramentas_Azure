# Passo a passo para a criação de um recurso no Azure Machine Learning

---

Com a conta do Azure criada será necessário iniciar e criar um recurso no menu a esquerda da tela. 

![download](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/07a7fb07-5acf-464f-8e61-a0dfe501c130)

Em seguida buscar por Azure Machine Learning, uma forma fácil de encontrar é pesquisar na barra de pesquisa pela ferramente. 

![download (1)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/afc0edbd-82fb-41fc-b6e0-d9c7dc775c7c)

Ao encontrar a ferramenta, clique em "Create" para iniciar a configuração do recurso. 
São várias as etapas para a configuração do recurso, sendo assim basta seguir os passos a seguir.
Em Subscrição será apresentado uma identificação do usuário, como um CPF do usuário dentro da conta. Por padrão, a Azure preenche esse campo de forma automática, não sendo necessário alterar. 

Logo em seguida, informe qual será o Recource Group, que é como uma basta organizadora para que os recursos criados não fiquem soltos na plataforma, permitindo uma maior facilidade em localizar os recursos criados. 
No primeiro acesso, será necessário criar um Recource Group e dar um nome. 
Em seguida, informe um nome para o projeto que é exclusivo. Em seguida a região, para o projeto foi utilizado a East US. 

Os demais campos de Storage account, Key vault e Application inseghts foram preenchidos automaticamente pela ferramenta e não sofreram alterações, eles são um local de organização do HD, local onde se inclui as chaves e certificados e uma identificação da aplicação respectivamente.

Para as demais configurações não sofreram alteração, porem para compreender cada etapa, temos:
Aba de Network com as permissões de acesso como publico e restrito, aba de Encryption com as questões de criptografia, Identity com informações de RBAC e permissionamento, Tags são os rótulos adicionados para os recursos, pois ajuda a rastreabilidade e depois no rateio dos gastos de cada recurso. 
Com essa primeira parte configurada, o Azure irá validar as informações para então criarmos o modelo. 

![download (2)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/2020ae51-d67e-4faa-970b-e11f8667def8)


Para configurar o modelo, após a finalização do processo e atualização do status do recurso para "Concluído".

![download (3)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/4eb17f9c-86db-4f7d-a3fe-f0ab858dfbe9)


No menu a esquerda em "Tarefas(Jobs)", abriremos o recurso e em seguida vamos clicar no botão de "+ Modelo de registro". Essa etapa é muito importante para a possibilidade de validarmos o modelo assim como ver suas métricas posteriormente. 

![download (4)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/7937caac-b3b2-4577-b25a-3b882a6b0d57)

Na criação do modelo, basta informar o tipo do modelo que pode ser MLflow, Triton ou Não especificado. Assim como adicionar um nome e descrição. 

A criação de um modelo é importante para validar as métricas do recurso criado.  Com o modelo criado, no menu a esquerda clique em "Tarefas(Job)" e em seguida escolha o recurso criado. Na tela apresentada iremos em métricas ver os gráficos residuais e o predicted que vão trazer a diferença entre o valor previsto e o valor real, comparando os valores.

![download (5)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/bc2a3531-0109-48de-85f9-1efcbb25007f)


Após a criação do modelo, será criado um Ponto de Extremidade indo no menu e clicando em Pontos de Extremidade e em seguida em "Criar". O Azure irá solicitar para qual modelo esse ponto de extremidade fará parte, basta selecionar o modelo e implantar. Para a a atividade não realizei nenhuma alteração de parâmetros nos campos de configuração do ponto de extremidade.

![download (6)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/9063fba7-194f-4c51-b0dd-e64f0c198089)


A criação de um Ponto de Extremidade pode demorar alguns minutos. 
A conferência das métricas do ponto de extremidade é feita na aba de modelos, no qual será apresentado o ponto de extremidade criado no passo anterior. Clique sobre para verificar as métricas, realizar validações e testes do modelo. 

![download (7)](https://github.com/gabriellivieira/Ferramentas_Azure/assets/112736236/ee262ad8-e169-40f3-9ff6-a74f95c00ec7)

Após a finalização da atividade, os recursos foram excluídos da conta Azure para não consumir mais créditos.

## Links uteis

Passo a passo detalhado Microsoft
* [Explore Automated Machine Learning in Azure Machine Learning](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html)

* [Explore Azure AI Services](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/02-content-safety.html)