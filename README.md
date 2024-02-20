# PROJETO: Análise de Sentimentos por Inteligência Artificial com Language Studio da Microsoft Azure AI.

Em uma análise verbal, cada frase é um quebra-cabeça, e cada palavra é uma peça essencial.



Com o Language Studio você dá todas as ferramentas para uma máquina desvendar o real sentido de algo que foi comunicado. Vocẽ aprimora sua aplicação para entender o que o emissor realmente quer transmitir, ou quais foram os tópicos principais de um texto, ou se ele transmitiu posicionamentos positivos, negativos ou neutros.



Olá! Me chamo Isac Freitas, e aqui vou demonstrar o uso da ferramenta Language Studio da Microsoft Azure AI para fazer análise de textos e extrair informações tais como: análise de sentimentos (satisfação), palavras-chave, frases-chave e outros.



Vou apresentar brevemente a ferramenta, usando de textos-exemplo para demostrar algumas das funcionalidades do Language Studio da Microsft Azure ML.

--------------------------

### Parte 1- Criação de um recurso de linguagem no portal da Azure.

--------------------------

Antes de usarmos as ferramentas do Language Studio, precisamos criar um recurso no portal da Azure para ser utilizado.



Pra criarmos o recurso, vamos entrar em "https://www.portal.azure.com" e clicar em "Criar um recurso".
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Analise-de-Sentimentos-por-Inteligencia-Artificial-com-Language-Studio/assets/65254733/cd98c54b-9be4-4915-8e7d-d099ab9d4067" width="800px" />
</div>

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

### Parte 2- Análise de Sentimentos no Language Studio.

--------------------------

Entramos em "https://language.cognitive.azure.com/"



Obrigado por me acompanhar nestes testes até aqui!

--------------------------

Então é isso.

# Este foi o meu primeiro projeto de Language Studio da Microsoft Azure ML, em meus estudos em Ciência de Dados.

Obrigado pela atenção!

**Qualquer dúvida sobre o projeto, ou caso precise de auxílio, fico a disposição. Entre em contato comigo por meio de minhas redes sociais (listadas abaixo ou em meu perfil).

--------------------------

Sobre mim:
# Isac Freitas
Estudante de Ciência de Dados e Inteligência Artificial.

### Me encontre:

Insta: @isac.sfreitas



Twitter: @isaczeitgeist
