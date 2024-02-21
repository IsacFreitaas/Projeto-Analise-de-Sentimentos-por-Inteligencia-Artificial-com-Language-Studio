# PROJETO: Análise de Sentimentos por Inteligência Artificial com Language Studio da Microsoft Azure AI.

Em uma análise verbal, cada frase é um quebra-cabeça, e cada palavra é uma peça essencial.



Com o Language Studio você dá todas as ferramentas para uma máquina desvendar o real sentido de algo que foi comunicado. Vocẽ aprimora sua aplicação para entender o que o emissor realmente quer transmitir, ou quais foram os tópicos principais de um texto, ou se ele transmitiu posicionamentos positivos, negativos ou neutros.



Olá! Me chamo Isac Freitas, e aqui vou demonstrar o uso da ferramenta Language Studio da Microsoft Azure AI para fazer análise de textos e extrair informações tais como: análise de sentimentos (satisfação), palavras-chave, frases-chave e outros. Hoje iremos testar somente a parte de análise de sentimentos.



Vou apresentar brevemente a ferramenta, usando de textos-exemplo para demostrar algumas das funcionalidades do Language Studio da Microsft Azure ML.

--------------------------

### Parte 1- Criação de um recurso de linguagem no portal da Azure.

--------------------------

Antes de usarmos as ferramentas do Language Studio, precisamos criar um recurso no portal da Azure para ser utilizado. Para isso, você precisa ter uma conta Microsft.



Pra criarmos o recurso, vamos entrar em "https://www.portal.azure.com" e clicar em "Criar um recurso".
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/cd98c54b-9be4-4915-8e7d-d099ab9d4067" width="800px" />
</div>

Vai ser aberto a parte de Criar recurso, na parte de Marketplace do portal da Azure.



Aqui, vamos na caixa de pesquisa e procuramos por "Language Services" (ou "Análise de Texto").
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/46da220c-0f9e-4e7d-8e05-fa60f9205918" width="800px" />
</div>

Clicamos em "Criar", nessa primeira opção que aparece, e "Análise de texto".
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/b8da2b83-e9be-4bf3-9c32-187e9b939c55" width="800px" />
</div>

Em "Select additional features", não precisa marcar nada, somente clicar em "Continue to create your resource".
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/49b4a52a-740f-4621-a0a6-7e75b787cd36" width="800px" />
</div>

Na caixinha de Grupo de recursos, você seleciona um grupo existente ou cria um novo para ser usado nesse projeto. No meu caso, irei criar um novo e chamar de "LanguageStudioLAB".
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/0933314b-4398-4087-b1d2-d2626f8ac3a6" width="800px" />
</div>

Descendo mais um pouco a página, aqui vamos selecionar a região do servidor que desejamos usar, o nome desse novo recurso e o tipo de preço que desejamos.



Vou deixar a região como East US mesmo, pois os servidores americanos são melhores e mais baratos que os servidores brasileiros.



Vou deixar o nome do recurso como "LanguageStudioLABDIO", e o tipo de preço em "Free F0".

<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/eba3e7c6-5dbc-42e5-ad5c-ca17395bece5" width="800px" />
</div>

Após isso, descemos um pouco mais na página e marcamos a caixinha para declarar que aceita os temos de uso do aviso de uso reponsável de inteligência artificial, e clicamos em Examinar + Criar.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/7465bcec-d86f-4e91-a0d9-97a26df5bf07" width="800px" />
</div>

<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/a6b19847-980e-4953-b692-9a87c2f64e38" width="800px" />
</div>

Agora você espera terminar a execução de validação final e confere se preencheu tudo corretamente, então clica em Criar.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/682f42c3-6b1a-4f8b-9fc8-1d6b5d2df88d" width="800px" />
</div>


Então você espera alguns minutos até terminar a implantação finalizar. Após concluída, continuamos nosso projeto.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/b5196604-d46c-4012-acf4-87599e7c882b" width="800px" />
</div>

--------------------------

### Parte 2- Análise de Sentimentos (satisfação) no Language Studio.

--------------------------

Agora acessamos "https://language.cognitive.azure.com/". 



Aqui você precisará logar com sua conta Microsoft e depois selecionar o grupo de recursos e o recurso que criamos anteriormente.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/56e46715-f839-4ce6-a190-60d35ee00919" width="800px" />
</div>

Na página inicial do Language Studio, você vai na aba "Classify text", e na primeira opção ("Analyze sentiment and mine opinion") você clica em "Try it out".
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/417a0d11-9a00-4efe-9740-c02bb522c7cd" width="800px" />
</div>

--------------------------

Agora precisamos de um texto para ser analisado.



Para isso, vou pedir ao Chat GPT para criar um texto de opinião de um review de um produto comprado pela internet.



Vou pedir que de preferência, seja um review negativo sobre tal produto.



<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/4d14f57c-c6ae-4062-9ad1-42bb16982174" width="925px" />
</div>

--------------------------

Agora voltamos ao Language Studio, selecionamos o idioma do texto (caso peça, você também precisará selecionar o recurso que vocẽ deseja usar) e colamos o texto que desejamos usar a ferramenta para analisar.



Então descemos mais um pouco a página e marcamos a caixinha que confirmamos que temos ciência que esse Demo usará valores incluidos em nosso recurso da Azure,
e clicamos em "Run".

<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/1130df90-1d1c-4acb-b505-760fc4f4cf93" width="800px" />
</div>


Então, ao terminar de carregar, podemos ver os resultados do nosso experimento:
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/963b5024-8ae3-43e3-819b-265125688b6a" width="800px" />
</div>

*A ANÁLISE COMPLETA ESTARÁ NA PASTA "OUTPUT" JUNTAMENTE COM A SAÍDA EM JSON.

Obrigado por me acompanhar nestes testes até aqui!

--------------------------

Então é isso.

# Este foi o meu primeiro projeto de Language Studio da Microsoft Azure ML, em meus estudos em Ciência de Dados.

Obrigado pela atenção!

LINK para Documentação de Apoio:



1- https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-analysis.html



**Qualquer dúvida sobre o projeto, ou caso precise de auxílio, fico a disposição. Entre em contato comigo por meio de minhas redes sociais (listadas abaixo ou em meu perfil).

--------------------------

Sobre mim:
# Isac Freitas
Estudante de Ciência de Dados e Inteligência Artificial.

### Me encontre:

Insta: @isac.sfreitas



Twitter: @isaczeitgeist
