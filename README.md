Desafio de Projeto: Construindo um Esquema Conceitual para Banco de Dados

Objetivo

Desenvolver um esquema conceitual de banco de dados para um sistema realista, utilizando a abordagem profissional de modelagem de dados. O modelo deve seguir as melhores práticas de normalização e representação gráfica.


---

1. Definição do Projeto

Cenário: Sistema de Gerenciamento de Pedidos para um E-commerce

Uma empresa de e-commerce precisa de um banco de dados para armazenar e gerenciar informações sobre clientes, produtos, pedidos, pagamentos e entregas. O sistema deve garantir integridade, evitar redundâncias e facilitar consultas rápidas.


---

2. Requisitos do Sistema

2.1 Regras de Negócio

Cada cliente pode realizar múltiplos pedidos.

Cada pedido pode conter vários produtos.

Os produtos podem pertencer a uma ou mais categorias.

Os pedidos podem ter diferentes formas de pagamento.

Cada pedido tem um status (Ex: Pendente, Pago, Enviado, Entregue, Cancelado).

Os pagamentos podem ser parcelados.

Cada produto tem um estoque controlado.


2.2 Atores do Sistema

Clientes: Fazem pedidos e realizam pagamentos.

Administradores: Gerenciam produtos e estoques.

Transportadoras: Responsáveis pelas entregas.



---

3. Modelo Conceitual – DER (Diagrama Entidade-Relacionamento)

3.1 Entidades e Atributos

3.2 Relacionamentos

Um cliente pode fazer vários pedidos, mas um pedido pertence a um único cliente (1:N).

Um pedido pode ter vários produtos, e um produto pode estar em vários pedidos (N:N), criando a entidade ItemPedido.

Um pedido pode ter um ou mais pagamentos (1:N).

Um pagamento pode ser parcelado em várias parcelas (1:N).

Um pedido pode ter uma única entrega, mas uma entrega está vinculada a um único pedido (1:1).



---

4. Diagrama Entidade-Relacionamento (DER)

Para melhor visualização, o modelo conceitual será representado em um diagrama. Você pode construir este diagrama no MySQL Workbench, DBDesigner, Lucidchart ou Draw.io.


---

5. Normalização

1ª Forma Normal (1FN): Todos os atributos contêm valores atômicos, sem repetições de grupos de dados.

2ª Forma Normal (2FN): Todas as tabelas dependem totalmente de suas chaves primárias.

3ª Forma Normal (3FN): Nenhuma coluna depende transitivamente de outra que não seja a chave primária.



---
