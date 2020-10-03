# API REST com JSON SERVER

JSON Server é uma biblioteca capaz de criar uma API Fake em 30 segundos. Isso mesmo, em 30s.E o dev não precisa escrever nenhuma linha de código.

**Passo a Passo:**
1 - Instale o Json Server: npm install -g json-server

2 - Crie um arquivo .json(eu utilizei um que já tinha de um exercício anterior)

3 - Inicie o servidor: npm dev server
Obs.: Esse comando foi possivel, pois no meu package.json, após dar "npm init" e realizar instalação do json-server,
acrescentei essa linha, no package.json: 
 "dev": "json-server --watch games.json --port 3000"

4 - Ao iniciar o servidor, agora é brincar com as ROTAS:
GET:          http://localhost:3000/games
GET(ID):  http://localhost:3000/games/1070
POST: Salvar um game
PUT(Id): Atualizar um game
PATCH(ID): Atualizar parte da descrição de um games
DELETE(ID): Remove um game

Lembrando que as rotas é acessada pelo endereço base, ou seja: http://localhost:3000/
Existe ferramentas como: Postman e Insomnia, para verificar e manipular as requisições desejadas!! 

Dois Exemplos para brincar:
Podemos usar os filtros:
http://localhost:3000/games?genre=Puzzle

Podemos ordenar, até de forma descendente:
http://localhost:3000/games?_sort=name&amp;_order=desc

 

Fonte: [https://github.com/typicode/json-server]


 
 