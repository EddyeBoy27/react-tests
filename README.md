# Boas vindas ao repositório do projeto de Testes em React!

## O que foi desenvolvido

Este repositório já contém um _template_ de uma aplicação React criado e configurado. Foi utilizado [`Jest`](https://jestjs.io/) e a biblioteca [`React Testing Library`](https://testing-library.com/) (também já instaladas e configuradas) para escrever os testes. Note que o _template_ contém uma implementação completa de todos os requisitos da Pokédex. Para cada requisito ou sub-requisito do projeto, foi escrito ao menos um teste que garanta sua corretude.

---

## Requisitos do projeto

### 1 - Ao carregar a aplicação no caminho de URL “/”, a página principal da Pokédex deve ser mostrada.

### 2 - A Pokédex deve exibir apenas um pokémon por vez

### 3 - Ao apertar o botão de próximo, a página deve exibir o próximo pokémon da lista

  - O botão deve conter o texto `Próximo pokémon`;

  - Cliques sucessivos no botão devem mostrar o próximo pokémon da lista;

  - Ao se chegar ao último pokémon da lista, a Pokédex deve voltar para o primeiro pokémon no apertar do botão.

### 4 - A Pokédex deve conter botões de filtro

  - A partir da seleção de um botão de tipo, a Pokédex deve circular somente pelos pokémons daquele tipo;

  - O texto do botão deve ser o nome do tipo, p. ex. `Psychic`.

### 5 - A Pokédex deve conter um botão para resetar o filtro

  - O texto do botão deve ser `All`;

  - Após clicá-lo, a Pokédex deve voltar a circular por todos os pokémons;

  - Quando a página carrega, o filtro selecionado deve ser o `All`.

### 6 - A Pokédex deve gerar, dinamicamente, um botão de filtro para cada tipo de pokémon

  - Os botões de filtragem devem ser dinâmicos: sua Pokédex deve gerar um botão de filtragem para cada tipo de pokémon disponível nos dados independente de quais ou quantos sejam, sem repetição de tipos. Ou seja, se sua Pokédex possui pokémons do tipo `Fire`, `Psychic`, `Electric` e `Normal`, deve aparecer como opção de filtro um botão para cada um desses tipos. Além disso, ela deve manter o botão `All`.

### 7 - O botão de `Próximo pokémon` deve ser desabilitado se a lista filtrada de pokémons tiver um só pokémon

### 8 - A Pokedéx deve exibir o nome, tipo, peso médio e imagem do pokémon exibido

  - O peso médio do pokémon deve ser exibido com um texto no formato `Average weight: <value> <measurementUnit>`, onde `<value>` e `<measurementUnit>` são, respectivamente, o peso médio do pokémon e sua unidade de medida;

  - A imagem deve conter um atributo `src` com a URL da imagem do pokémon. A imagem deverá ter também um atributo `alt` com o nome do pokémon.

### 9 - O pokémon exibido na Pokedéx deve conter um link de navegação para exibir detalhes deste pokémon

  - O link deve possuir a URL `/pokemons/<id>`, onde `<id>` é o id do pokémon exibido.

### 10 - Ao clicar no link de navegação do pokémon, a aplicação deve ser redirecionada para a página de detalhes de pokémon

  - A URL exibida no navegador deve mudar para `/pokemon/<id>`, onde `<id>` é o id do pokémon cujos detalhes se deseja ver.

### 11 - A página de detalhes de pokémon deve exibir o nome, tipo, peso médio e imagem do pokémon exibido

  - O peso médio do pokémon deve ser exibido com um texto no formato `Average weight: <value> <measurementUnit>`, onde `<value>` e `<measurementUnit>` são, respectivamente, o peso médio do pokémon e sua unidade de medida;

  - A imagem deve conter um atributo `src` com a URL da imagem do pokémon. A imagem deverá ter também um atributo `alt` com o nome do pokémon.

### 12 - O pokémon exibido na página de detalhes não deve conter um link de navegação para exibir detalhes deste pokémon

### 13 - A página de detalhes deve exibir uma seção com um resumo do pokémon

  - A seção de detalhes deve conter um heading `h2` com o texto `Summary`;

  - A seção de detalhes deve conter um parágrafo com o resumo do pokémon específico sendo visualizado.

### 14 - A página de detalhes deve exibir uma seção com os mapas com as localizações do pokémon

  - A seção de detalhes deve conter um heading `h2` com o texto `Game Locations of <pokémon>`, onde `<pokémon>` é o nome do pokémon exibido;

  - A seção de detalhes deve exibir todas as localizações do pokémon;

  - Cada localização deve exibir o nome da localização e uma imagem do mapa da localização;

  - A imagem da localização deve ter um atributo `src` com a URL da localização;

  - A imagem da localização deve ter um atributo `alt` com o texto `<name> location`, onde `<name>` é o nome do pokémon.

### 15 - A página de detalhes deve permitir favoritar um pokémon

  - A página deve conter um checkbox que permita favoritar um pokémon. Cliques no checkbox devem, alternadadamente, adicionar e remover o pokémon da lista de favoritos;

  - O label do checkbox deve ser `Pokémon favoritado?`.

### 16 - Pokémons favoritados devem exibir um ícone de uma estrela

  - O ícone deve ser uma imagem, com o atributo `src` igual `/star-icon.svg`;

  - A imagem deve ter o atributo `alt` igual a `<pokemon> is marked as favorite`, onde `<pokemon>` é o nome do pokémon cujos detalhes estão sendo exibidos.

### 17 - No topo da aplicação, deve haver um conjunto fixo de links de navegação

  - O primeiro link deve possuir o texto `Home` com a URL `/`;

  - O segundo link deve possuir o texto `About` com a URL `/about`;

  - O terceiro link deve possuir o texto `Favorite Pokémons` com a URL `/favorites`.

### 18 - Ao clicar no link "Home" na barra de navegação, a aplicação deve ser redirecionada para a página inicial, na URL "/"

### 19 - Ao clicar no link "About" na barra de navegação, a aplicação deve ser redirecionada para a página de `About`, na URL "/about"

### 20 - Ao clicar no link "Favorite Pokémons" na barra de navegação, a aplicação deve ser redirecionada para a página de pokémons favoritados, na URL "/favorites"

### 21 - A página "About" deve exibir informações sobre a Pokédex

  - A página deve conter um heading `h2` com o texto `About Pokédex`;

  - A página deve conter dois parágrafos com texto sobre a Pokédex;

  - A página deve conter a seguinte imagem de uma Pokédex: `https://cdn.bulbagarden.net/upload/thumb/8/86/Gen_I_Pok%C3%A9dex.png/800px-Gen_I_Pok%C3%A9dex.png`.

### 22 - A página de pokémon favoritos deve exibir os pokémons favoritos

  - A página deve exibir todos os pokémons favoritados;

  - A página não deve exibir nenhum pokémon não favoritado.

### 23 - Entrar em uma URL desconhecida exibe a página `Not Found`

  - A página deve conter um heading `h2` com o texto `Page requested not found 😭`;

  - A página deve exibir a imagem `https://media.giphy.com/media/kNSeTs31XBZ3G/giphy.gif`.

### 24 - A cobertura de testes deve ser 100%

  - Para ver a cobertura de testes, execute no terminal o comando `npm run test-coverage`.