# Cad-Ecommerce Project

**𝐍𝐨𝐰 𝐥𝐨𝐚𝐝𝐢𝐧𝐠...**

---

## Índice 🗝️

- [Descrição](#descrição)
- [Introdução](#introdução)
- [Funcionalidades](#funcionalidades)
- [Códigos](#códigos)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Métodos PHP Utilizados](#métodos-php-utilizados)
- [Exemplos Auxiliares](#exemplos-auxiliares)
- [Banco de Dados](#banco-de-dados)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Fontes Consultadas](#fontes-consultadas)
- [Autores](#autores)

### Descrição

Este projeto é uma aplicação de e-commerce que permite aos usuários navegar por produtos, adicionar itens ao carrinho, realizar pedidos e cadastrar novos produtos e clientes. A aplicação é desenvolvida utilizando PHP para o backend, com um banco de dados MySQL, e uma interface web simples usando HTML, CSS e JavaScript.

### Introdução

A aplicação de e-commerce foi criada para facilitar o processo de compra online. Ela permite que os usuários naveguem por diferentes produtos, adicionem produtos ao carrinho, visualizem o resumo do pedido e finalizem suas compras. Além disso, a aplicação oferece funcionalidades de cadastro para produtos, categorias, marcas e clientes.

### Funcionalidades

1. **Visualização de Produtos:** Exibe uma lista de produtos com informações detalhadas.
2. **Carrinho de Compras:** Permite adicionar e remover produtos do carrinho.
3. **Finalização de Pedido:** Permite a finalização do pedido e atualização do estoque.
4. **Cadastro de Produtos:** Interface para adicionar novos produtos ao banco de dados.
5. **Cadastro de Categorias e Marcas:** Interface para cadastrar novas categorias e marcas.

### Códigos

- **`controller/carrinho-add.php`**
  - **Descrição:** Adiciona um produto ao carrinho. Usa a classe `Carrinho` e seu método `add()`.

- **`controller/carrinho-busca.php`**
  - **Descrição:** Busca e exibe os produtos no carrinho. Usa a classe `Carrinho` e seu método `buscar()`.

- **`controller/carrinho-remover.php`**
  - **Descrição:** Remove um produto do carrinho. Usa a classe `Carrinho` e seu método `remover()`.

- **`controller/conexao.php`**
  - **Descrição:** Estabelece a conexão com o banco de dados MySQL.

- **`controller/produtos-busca.php`**
  - **Descrição:** Busca e exibe produtos disponíveis. Usa a classe `Produtos` e seu método `buscar()`.

- **`controller/produtos-pedido.php`**
  - **Descrição:** Finaliza o pedido e atualiza o estoque. Usa a classe `Produtos` e seu método `pedido()`.

- **`controller/produtos-resumo.php`**
  - **Descrição:** Exibe o resumo do pedido. Usa a classe `Produtos` e seu método `resumo()`.
 
  #### Model

- **`cadMarca.php`**
  - **Descrição:** Cadastro de marcas.

- **`Carrinho.class.php`**
  - **Descrição:** Este arquivo contém a classe `Carrinho` que gerencia o carrinho de compras. Inclui métodos para adicionar, buscar e remover produtos do carrinho.

- **`Produtos.class.php`**
  - **Descrição:** Este arquivo contém a classe `Produtos` que gerencia a busca e exibição de produtos, além de gerenciar pedidos. Inclui métodos para buscar produtos, finalizar pedidos e gerar resumos.
 
  ### Banco de Dados

A estrutura do banco de dados é composta por tabelas que armazenam informações sobre produtos, categorias, marcas, clientes, pedidos e itens do pedido.

#### Estrutura das Tabelas

- **Produtos**
  - **IDPROD:** Identificador do produto.
  - **NOME:** Nome do produto.
  - **DESCRICAO:** Descrição do produto.
  - **PRECO:** Preço do produto.
  - **ESTOQUE:** Quantidade em estoque.
  - **IDCATEGORIA:** Identificador da categoria do produto.
  - **IDMARCA:** Identificador da marca do produto.
 
  - **Categoria**
  - **IDCATEGORIA:** Identificador da categoria.
  - **DESCRICAO:** Descrição da categoria.











