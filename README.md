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
    
 
- **Marca**
  - **IDMARCA:** Identificador da marca.
  - **DESCRICAO:** Descrição da marca.
 
  
- **Cliente**
  - **IDCLI:** Identificador do cliente.
  - **NOME:** Nome do cliente.
  - **EMAIL:** E-mail do cliente.
 
- **Pedido**
  - **IDPED:** Identificador do pedido.
  - **IDCLI:** Identificador do cliente que realizou o pedido.
  - **IDFOR:** Identificador do fornecedor.
  - **STATUS:** Status do pedido.
 
- **Itens**
  - **IDITEM:** Identificador do item.
  - **IDPED:** Identificador do pedido.
  - **IDPROD:** Identificador do produto.
  - **QNT:** Quantidade do produto.


### Tecnologias Utilizadas

O projeto utiliza as seguintes tecnologias:

- **PHP:** Linguagem de programação para a lógica do servidor.
- **MySQL:** Sistema de gerenciamento de banco de dados.
- **HTML/CSS:** Markup e estilo para o front-end.
- **JavaScript/jQuery:** Para interatividade e manipulação do DOM.

### Estrutura do Projeto

O projeto está organizado da seguinte forma:

#### Pasta `controller`

Esta pasta contém os arquivos responsáveis pelo controle das operações do carrinho e dos produtos.

- **carrinho-add.php**
- **carrinho-busca.php**
- **carrinho-remover.php**
- **conexao.php**
- **produtos-busca.php**
- **produtos-pedido.php**
- **produtos-resumo.php**


#### Pasta Geral  `CADECOMMERCE`

Esta pasta contém os arquivos principais do sistema.

- **carrinho.php**
- **categoria.php**
- **indice.php**
- **inserir-categoria.php**
- **inserir-marca.php**
- **inserir-produto.php**
- **marca.php**
- **pedido.php**
- **produtos.php**

### Métodos PHP Utilizados

- **`mysqli_connect`**: Estabelece uma conexão com um servidor MySQL.
- **`mysqli_query`**: Executa uma consulta no banco de dados.
- **`mysqli_fetch_assoc`**: Retorna uma linha de resultado como uma matriz associativa.
- **`mysqli_close`**: Fecha a conexão com o banco de dados.

#### Exemplos Auxiliares

##### Cadastro de Categoria

- **categoria.php:** Formulário para cadastro de categorias.
- **insere-categoria.php:** Código PHP para inserir uma nova categoria no banco de dados.

##### Cadastro de Marca

- **marca.php:** Formulário para cadastro de marcas.
- **insere-marca.php:** Código PHP para inserir uma nova marca no banco de dados.

##### Cadastro de Produto

- **produtos.php:** Formulário para cadastro de produtos.
- **insere-produto.php:** Código PHP para inserir um novo produto no banco de dados.

### Comentários no Código

Todos os arquivos PHP neste projeto contêm comentários explicando as funcionalidades inovadoras. Esses comentários ajudam na compreensão do fluxo do código e na manutenção futura.

### Fontes Consultadas

- [Inteligência Artificial](https://chat.openai.com/)
- [Alura](https://www.alura.com.br/artigos/escrever-bom-readme)
- [Documentação PHP](https://www.php.net/manual/pt_BR/)
- [Documentação MySQL](https://dev.mysql.com/doc/)
- [jQuery Documentation](https://jquery.com/)






















