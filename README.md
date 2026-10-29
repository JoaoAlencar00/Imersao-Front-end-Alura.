# Imersão Front-end — Interface de Música

Projeto educacional desenvolvido durante a Imersão Front-end da Alura. A interface é inspirada no Spotify e combina HTML, CSS e JavaScript com uma consulta a uma API local de artistas.

## Recursos

- Navegação lateral e apresentação de playlists.
- Campo de pesquisa que consulta artistas por nome.
- Exibição de nome e imagem do artista retornado pela API.

## Tecnologias

HTML5, CSS3, JavaScript, Fetch API e um arquivo JSON para simulação dos dados.

## Como executar

É necessário ter Git, Node.js e npm disponíveis para iniciar a API de demonstração.

```bash
git clone https://github.com/JoaoAlencar00/Imersao-Front-end-Alura..git imersao-frontend
cd imersao-frontend
npx json-server@0.17.4 --watch api-artists/artists.json --port 3000
```

Mantenha esse processo em execução e abra `index.html` em um navegador, preferencialmente por um servidor estático como Live Server.

A versão 0.17.4 do JSON Server mantém o filtro `name_like` usado em `script.js`. A API é consultada em `http://localhost:3000/artists`. Veja a [documentação dessa versão](https://github.com/typicode/json-server/tree/v0.17.4).

## Estrutura

- `index.html`: interface.
- `script.js`: consulta e apresentação dos resultados.
- `api-artists/artists.json`: dados de artistas.
- `src/styles/`: estilos carregados pela página.
- `src/assets/`: recursos visuais.

## Escopo

O projeto simula uma busca com dados locais. Não integra a API oficial do Spotify nem implementa streaming ou autenticação. O tratamento de falhas da API e de buscas sem resultados permanece como oportunidade de evolução.

Projeto de estudo da Alura. Spotify e os demais recursos visuais pertencem aos respectivos titulares.
