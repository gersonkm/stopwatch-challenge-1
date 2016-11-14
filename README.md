#Exercício

Os participantes deverão desenvolver uma aplicação web capaz de fazer pesquisas sobre filmes catalogados no site 'The Movie Database'.

###Funcionalidades

As seguintes funcionalidades deverão estar presentes na aplicação:

1. Uma interface web com um campo texto para digitar o título do filme e um botão para acionar a pesquisa.
2. O usuário poderá digitar parte do **título original** de um filme ou parte dos **títulos traduzidos** para outros idiomas.
3. O resultado da pesquisa, que deverá ser limitado em 20 filmes, apresentará as seguintes informações: 
    1. título original do filme
	1. gênero  do filme (em português)
	1. ano de lançamento do filme
	1. sinopse do filme (em português)
	1. imagem do cartaz do filme
4. O botão de pesquisa poderá ser acionado ao pressionar a tecla 'ENTER' no campo de busca. 
5. Quando o filme não tiver uma imagem de cartaz, deverá mostrar uma outra imagem do mesmo tamanho (154 x 231) no lugar.  

###Requisitos técnicos
1. Utilizar a versão 3 do ['The Movie Database (TMDb) API'](https://www.themoviedb.org/documentation/api).
2. Utilizar a API key (v3 auth) que será enviada por e-mail aos participantes.
3. Não é permitido usar qualquer wrapper sobre a API do TMDb.
4. A aplicação deverá ser escrita na linguagem Java.
5. Não é permitido adicionar qualquer biblioteca externa no projeto.

###Dicas
1. Para pesquisar os filmes, use o endpoint `GET https://developers.themoviedb.org/3/search/search-movies`.
2. Para obter os elencos de um filme, use o endpoint `GET /movie/{movie_id}/credits` (consulte a documentação).
3. Para obter os gêneros, use o endpoint `GET /genre/movie/list`.
4. Para obter as imagens dos cartazes, utilize a URI base `http://image.tmdb.org/t/p/w154`. 
5. No site da documentação oficial, utilize a aba 'try it out' para testar as chamadas da API. 
6. Para iterar sobre um array dentro do template handlebars, utilize o [each block helper](http://handlebarsjs.com/builtin_helpers.html).

###Atenção 
A lista de funcionalidades e a lista dos requisitos técnicos podem ser alteradas a qualquer momento. 
