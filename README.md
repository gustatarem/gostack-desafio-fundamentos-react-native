<img alt="GoStack" src="https://storage.googleapis.com/golden-wind/bootcamp-gostack/header-desafios-new.png" />

<h3 align="center">
  Desafio 08: Fundamentos do React Native
</h3>

## :rocket: Sobre o desafio

O GoMarketplace é uma aplicação desenvolvida usando React Native junto com o TypeScript, utilizando rotas, Async Storage e a Context API, que simula um e-commerce de forma simples, utilizando adição e remoção de itens a um carrinho e calculando o valor total de uma compra.

## :warning: Utilizando uma fake API

Antes de tudo, para que você tenha os dados para exibir em tela, criamos um arquivo que você poderá utilizar como fake API para te prover esses dados.

Para isso, deixamos instalado no seu package.json uma dependência chamada `json-server`, e um arquivo chamado `server.json` que contém os dados para uma rota `/products`. Para executar esse servidor você pode executar o seguinte comando:

```js
  yarn json-server server.json -p 3333
```

## :trophy: Funcionalidades da aplicação

- **`Listar os produtos da fake API`**: A página `Dashboard` exibe uma listagem através de uma tabela, com os campos `title`, `image_url` e `price`.

- **`Adicionar itens ao carrinho`**: Utilizando o Contexto chamado `cart` é possível adicionar itens ao carrinho através da Dashboard.

- **`Exibir itens do carrinho`**: A página `Cart` exibe todos os itens do carrinho, junto com a quantidade, valor único, valor subtotal dos itens e total de todos os itens.

- **`Aumentar quantidade de itens do carrinho`**: Em su página `Cart` permite que o usuário aumente a quantidade de itens do mesmo produto utilizando a função `increment` dentro do seu contexto em `/src/hooks/cart.tsx`.

**Dica**: Ao editar um item, quando for envia-lo para o backend, lembre de copiar os dados anteriores como o `available` e o `id`, ou eles serão  perdidos do seu arquivo server.json.

- **`Diminuir quantidade de um item do carrinho`**: Em suapágina `Cart` permite que o usuário decremente a quantidade de itens do mesmo produto utilizando a função `decrement` dentro do seu contexto em `/src/hooks/cart.tsx`.

**Dica**: Após; remover o item da sua API, lembre-se de remover ele também da listagem.
- **`Exibir valor total dos itens no carrinho`**: Tanto na página `Dashboard`, quanto na página `Cart` é poss' visualizar o valor total de todos os itens que estão no seu carrinho.

## :computer: Instruções de instalação e teste

Clone o repositório usando o `git` ou faça o download no formato zip. 
Antes de tudo, certifique-se de que você tem um gerenciador de pacotes (como o yarn) e o `Node.js` instalados em sua máquina.

Após baixar o projeto, abra uma aba do terminal e execute os seguintes comandos:

```Bash
# ../pasta-de-destino
$ cd gostack-desafio-fundamentos-react-native
# ../pasta-de-destino/gostack-desafio-fundamentos-react-native
$ yarn
```

Caso esteja usando macOS e vá rodar o app no iOS Simulator ou em um iPhone:

```Bash
# ../pasta-de-destino/gostack-desafio-fundamentos-react-native
$ cd ios
# ../pasta-de-destino/gostack-desafio-fundamentos-react-native/ios
$ pod install
```

Para iniciar a aplicação no iOS:

```Bash
# ../pasta-de-destino/gostack-desafio-fundamentos-react-native
$ yarn ios
```

Para iniciar a aplicação no Android:

```Bash
# ../pasta-de-destino/gostack-desafio-fundamentos-react-native
$ yarn android
```

Para rodar os testes da aplicação:

```Bash
# ../pasta-de-destino/gostack-desafio-fundamentos-react-native
$ yarn test
```
