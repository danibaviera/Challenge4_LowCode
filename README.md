# Tech Challenge 4 - Low Code Outsystems

## Descrição do Projeto
Este projeto foi desenvolvido como parte do **Tech Challenge 4**, utilizando a plataforma **Outsystems**. O sistema implementado é um **controle de estoque**, com funcionalidades para gerenciar produtos e suas movimentações, garantindo que as informações estejam sempre atualizadas.

## Funcionalidades
1. **Tela de Login**:
   - Apresenta a proposta do projeto.
   - Mensagem de boas-vindas ao sistema de estoque.
   - Login com usuário e senha para acesso seguro.

2. **Listagem de Produtos**:
   - Exibe o nome, valor e quantidade de produtos cadastrados no estoque.
   - Permite navegação para outras funcionalidades.

3. **Adicionar Produto**:
   - Tela para criar novos produtos.
   - Após o cadastro, os produtos aparecem na listagem inicial do estoque.

4. **Movimentação de Estoque**:
   - Tela acessada pelo menu superior.
   - Permite a edição do estoque por meio de movimentações.
   - Funcionalidade para entrada ou saída de produtos:
     - **Entrada**: Adiciona ao estoque.
     - **Saída**: Remove do estoque.
   - Atualiza automaticamente os valores na tela de Produtos.

## Estrutura Técnica

### Organização do Projeto
O projeto foi dividido em dois módulos principais:
- **Backend**
- **Frontend**

### Backend
1. **Entities - Database**:
   - **Tabela Produto**: Armazena os dados da listagem inicial do estoque.
   - **Tabela Movimentação**: Gerencia o fluxo de movimentações no estoque, vinculando dados através de IDs.
   - **Tabela Tipo de Movimentação**: Define o tipo de movimentação (entrada ou saída) para controle do fluxo de estoque.

2. **Lógica e Integrações**:
   - Configurada para gerenciar as interações entre banco de dados e interface.

### Frontend
1. **Interface - UI Flows**:
   - No **MainFlow**, foram criados fluxos e lógicas para integração das telas e banco de dados.
   - Telas implementadas:
     - **Produtos**: Tela inicial do sistema, considerada a Home.
     - **ProdutosDetail**: Exibe detalhes de um produto específico.
     - **Movimentacaos**: Tela que lista as movimentações do estoque.
     - **MovimentacaoDetail**: Permite adicionar ou visualizar detalhes de uma movimentação.

### Fluxo de Funcionalidades
- **Tela de Login** → **Home (Produtos)** → **Adicionar Produto**.
- **Home (Produtos)** → **Movimentação (Edição de Estoque)** → **Atualização da Listagem de Produtos**.

## Como Executar
1. **Requisitos**:
   - Plataforma Outsystems instalada.
   - Projeto importado para o ambiente.

2. **Passos**:
   - Abra o projeto **ControleEstoque**.
   - Certifique-se de que as tabelas e os fluxos foram configurados corretamente.
   - Execute a aplicação para acessar as telas e funcionalidades descritas.

## Tecnologias Utilizadas
- **Outsystems**: Desenvolvimento Low Code.
- **Banco de Dados**: Configuração via Entities.
- **Frontend**: Criação de telas interativas usando o MainFlow.
