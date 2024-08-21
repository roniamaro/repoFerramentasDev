# repoFerramentasDev
Um repositório criado para armazenar os projetos desenvolvidos em aula.

# 1.Git e GitHub e Terminais do Linux e Windows

# 2.Regex

# 3.VSCode, Nginx e Swagger
  - VSCode:

  - Nginx:

  - Swagger:
  200 — OK: This is the standard response for successful HTTP requests. The actual meaning of the response depends on the request method used:
    GET: Resource obtained and is in the message body
    HEAD: Headers are included in the response
    POST or PUT: Resource describing the result of the action sent is in the message body
    TRACE: Message body contains the request message as received by the server
    201 — Created: The request succeeded and a new resource was created. This is usually the response after POST or PUT requests. 

  202 — Accepted: The request was accepted but is still in progress. It’s used for cases where another server handles the request or for batch processing. 

  204 — No Content: The request was successfully processed, but there is no content. The headers may be useful. 

  400 — Bad Request: The server can’t or won’t process the request due to a client error. For example, invalid request message framing, deceptive request routing, size too large, etc.

  401 — Unauthorized: The user doesn’t have valid authentication credentials to get the requested resource.

  404 — Not Found: The server can’t find the requested resource, and no redirection has been set. 404 errors can harm your SEO efforts.

  408 — Request Timeout: The server timed out waiting because the client didn’t produce a request within the allotted time.

  413 — Payload Too Large: The client’s request is larger than the server’s defined limits, and the server refuses to process it.

  500 — Internal Server Error: The server has encountered an unexpected error and cannot complete the request.

  É possível rodar o Swagger Editor localmente pra isso precisamos usar em um servidor Docker:
    docker pull swaggerapi/swagger-editor
    docker run -d -p 80:8080 swaggerapi/swagger-editor

    docker run -d -p 80:8080 -v $(pwd):/tmp -e SWAGGER_FILE=/tmp/swagger.json swaggerapi/swagger-editor

  You can specify a different base url via BASE_URL variable for accessing the application - for example if you want the application to be available at http://localhost/swagger-editor/:
    docker run -d -p 80:8080 -e BASE_URL=/swagger-editor swaggerapi/swagger-editor

  É possível rodar também o Swagger UI localmente e disponibilizar aos clientes via Docker.

# 4.IA
  ## ChatGPT: desvendando a IA em conversas e suas aplicações
    Preparando o ambiente: antes de começar
    Link: https://chatgpt.com/
    User: login com Microsoft

    01. ChatGPT como gerador de texto
    >> Limites da IA
    Geração de texto, lista...
    Exemplo: Quero escrever uma lista de 7 hoteis em Campinas próximas a Lagoa do Taquaral:
    Transformar a resposta em um post:
    Exemplo: Transforme isso em um post. Quero um paragrafo por Lagoa do Taquaral, dizendo o ponto especial positivo dele. Use palavras intelectuais e chique. Seja breve e coloque uma introdução bacana e amigável. Finalize com uma chamada de vendas, do tipo "Não perca, compre agora".

    >> Localizações e viés
    É necessário especificar a localicação (cultural, regional, país) do que é solicitado.
    Exemplo: Liste 10 pessoas influentes do Jazz do Brasil para entrevistarmos em um podcast sobre Jazz.

    02. Trabalhando com textos e como o ChatGPT funciona
    >> Resumindo com IA
    É possível resumir matérias, textos, "links/podcast?".
    Exemplo: Resuma em 1 frase o texto abaixo: "Insira aqui o texto..."

    >> Como o ChatGPT funciona?
    É possível criarmos algo "novo/inédito", como uma poesia, um soneto...
    A IA busca e aprende de sua base de dados formas de gerar frases ineditas, porém é necessário manter um certo controle de qualidade e sempre verificar o que foi gerado.

    03. A IA vai tentar responder tudo!
    >> Controle de qualidade
    É possível implementar regras de validação no prompt.
    Exemplo: 
    Escreva o texto em primeira pessoal;
    Utilize paragrafos curtos;
    Exiba um botão de call to action ao final do texto;

    >> Portugês ou Inglês?
    
    04. Geradores de imagens e reflezão sobre inteligência.
    >> Stable Diffusion
    Os prompts são feitos por meio de palavras chave e inglês é bem melhor nessa situação para bolar o prompt.
    Prompt, é o que você quer na imagem;
    Negative promp, é o que você não quer na imagem;

    >>> Para saber mais:
    Stable Diffusion
    É capaz de gerar imagens fotorrealistas a partir de qualquer entrada de texto, cultiva liberdade autônoma para produzir imagens incríveis, capacita muitas pessoas para criar uma arte impressionante em segundos. O uso é gratuito e vale a pena conferir.

    Midjourney
    O Midjourney é executado no Discord e possui um servidor com canais para trabalho colaborativo, suporte técnico e de cobrança, anúncios oficiais, feedback e discussões. Ganhou uma grande notoriedade na comunidade por conta dos diferentes tipos de imagens geradas. Seu uso pago e neste link você encontra o valor da assinatura.

    PromptHero
    É um site incrível que divulga milhões de resultados de diferentes IAs, como Stable Diffusion e Midjourney, além de mostrar qual é a entrada que gerou cada imagem ou resultado. O uso é gratuito.

  ## ChatGPT e programação: aumente sua produtividade
    Objetivo:
    Entender algoritimos;
    Aprender conceitos;
    Encontrar bugs;
    Gerar códigos;

    Requisitos:
    Saber usar o ChatGPT;
    Programação (qualquer linguagem):
      API Rest;
      CRUD (Create, ead, Update, Delete);
      Banco de dados;

  ## ChatGPT: otimizando a qualidade dos resultados
  
  ## GitHub Copilot e ChatGPT: impulsionando seu desenvolvimento com IA