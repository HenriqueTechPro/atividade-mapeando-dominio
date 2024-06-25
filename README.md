# Sistema de Gerenciamento de Estoque

## Descrição

Este é um sistema de gerenciamento de estoque desenvolvido para ajudar a rastrear produtos, definir quantidades mínimas de estoque, receber alertas, visualizar histórico de vendas e estoque, e gerenciar ordens de compra.

## Entidades de Domínio

### Produto

- **Atributos**:
  - ID único
  - Nome
  - Quantidade em Estoque
  - Quantidade Mínima em Estoque
  - Tamanho
  - Cor
  - Histórico de Vendas
  - Fornecedor

### Estoque

- **Atributos**:
  - Produtos
  - Quantidades
  - Alertas
  - Histórico de Movimentações

### Histórico de Vendas

- **Atributos**:
  - Produto
  - Quantidade Vendida
  - Data da Venda
  - Lucro por Produto
  - Tendências de Venda

### Ordem de Compra

- **Atributos**:
  - ID
  - Produtos
  - Quantidades
  - Data de Criação
  - Status
  - Fornecedor
  - Prazo de Entrega

### Fornecedor

- **Atributos**:
  - ID
  - Nome
  - Informações de Contato
  - Atualizações sobre Prazos de Entrega

## Casos de Uso

### Rastrear Produto Individualmente

- Atribuir número de identificação único a cada produto
- Adicionar informações extras (tamanho, cor)
- Rastrear movimentações no estoque

### Definir Quantidades Mínimas de Estoque

- Configurar limite mínimo para cada produto
- Receber alertas quando o estoque estiver baixo

### Receber Alertas

- Configurar alertas por e-mail
- Configurar notificações no sistema de gerenciamento de estoque

### Visualizar Histórico de Vendas e Estoque

- Ver quantidades vendidas em um período
- Ver lucro gerado por produto
- Identificar produtos mais vendidos por período
- Observar tendências de estoque ao longo do tempo

### Gerenciar Ordens de Compra

- Criar ordens de compra automaticamente com base nas quantidades mínimas de estoque e tendências de vendas
- Gerenciar status das ordens de compra

### Integrar com Fornecedores

- Receber atualizações automáticas sobre prazos de entrega de novas remessas

## Requisitos

- [ ] Rastrear produtos individualmente com ID único e informações adicionais
- [ ] Definir e monitorar quantidades mínimas de estoque
- [ ] Receber alertas por e-mail e notificações no sistema
- [ ] Visualizar histórico de vendas e tendências de estoque
- [ ] Criar e gerenciar ordens de compra automaticamente
- [ ] Integrar com fornecedores para atualizações de prazos de entrega

## Tecnologias Utilizadas

- **Node.js**: Plataforma JavaScript para execução do código no servidor.
- **Fastify**: Framework web para Node.js, focado em performance e baixo overhead.
- **Prisma**: ORM (Object-Relational Mapping) para Node.js e TypeScript, utilizado para interagir com o banco de dados.
- **PostgreSQL**: Sistema de gerenciamento de banco de dados relacional, utilizado para armazenar os dados da aplicação.
