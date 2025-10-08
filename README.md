# LH Games

Este projeto foi gerado com o [Angular CLI](https://github.com/angular/angular-cli) versão 15.0.4.
## Descrição

LH Games é uma plataforma de e-commerce para a venda de jogos. A aplicação conta com uma página inicial que exibe os jogos em promoção, uma página de login e uma área restrita para administração dos produtos. O projeto utiliza o Angular para o front-end e o `json-server` para simular um back-end com um banco de dados de jogos em formato JSON.

## Funcionalidades

  * **Página Inicial:** Exibe um carrossel de banners e uma lista de jogos em promoção.
  * **Login:** Página de autenticação para acesso à área restrita.
  * **Área Restrita:**
      * Cadastro de novos jogos.
      * Listagem dos jogos cadastrados.
      * Atualização das informações dos jogos.
      * Exclusão de jogos.

## Tecnologias Utilizadas

  * **Angular:** Framework principal para o desenvolvimento da aplicação.
  * **Angular Material:** Componentes de UI para a construção da interface.
  * **Bootstrap:** Framework CSS para estilização e responsividade.
  * **JSON Server:** Para simular uma API RESTful com base em um arquivo JSON.
  * **TypeScript:** Superset do JavaScript que adiciona tipagem estática.

## Começando

Para executar o projeto localmente, siga os passos abaixo.

### Pré-requisitos

  * Node.js (versão compatível com o Angular 15)
  * Angular CLI (versão 15.0.4)

### Instalação

1.  Clone o repositório:
    ```bash
    git clone https://github.com/standbytheboy/lh_games_angular.git
    ```
2.  Navegue até o diretório do projeto:
    ```bash
    cd lh_games_angular
    ```
3.  Instale as dependências:
    ```bash
    npm install
    ```

### Servidor de Desenvolvimento

Execute o comando abaixo para iniciar o servidor de desenvolvimento do Angular:

```bash
ng serve
```

Acesse a aplicação em `http://localhost:4200/`. A aplicação será recarregada automaticamente se você alterar qualquer um dos arquivos de origem.

Para simular o back-end, inicie o `json-server` em um terminal separado:

```bash
json-server --watch dbgames.json
```

Isso iniciará um servidor na porta `3000` que servirá os dados do arquivo `dbgames.json`.

## Scripts Disponíveis

  * `ng serve`: Inicia o servidor de desenvolvimento.
  * `ng build`: Compila o projeto. Os artefatos da compilação são armazenados no diretório `dist/`.
  * `ng test`: Executa os testes unitários via [Karma](https://karma-runner.github.io).
  * `ng watch`: Compila o projeto em modo de desenvolvimento e observa as alterações nos arquivos.

## Estrutura do Projeto

```
lh_games_angular/
├── src/
│   ├── app/
│   │   ├── inicio/ (Página inicial)
│   │   ├── login/ (Página de login)
│   │   ├── menu/ (Componente de menu)
│   │   ├── restrito/ (Área de administração de produtos)
│   │   ├── rodape/ (Componente de rodapé)
│   │   ├── app-routing.module.ts
│   │   ├── app.component.ts
│   │   └── app.module.ts
│   ├── assets/ (Recursos estáticos como imagens)
│   ├── index.html
│   └── main.ts
├── dbgames.json (Banco de dados de jogos)
├── angular.json
├── package.json
└── ...
```
