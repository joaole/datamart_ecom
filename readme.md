**Desafio de Projeto de Data Warehouse: Análise de Vendas de E-commerce**

### **Objetivo**
Construir um Data Warehouse para uma análise abrangente de vendas de um e-commerce. O objetivo principal é permitir consultas e análises que forneçam insights sobre as vendas, os clientes e os produtos para otimizar estratégias de negócio.

---

### **Etapas do Projeto**

#### **1. Obter Dados Brutos**
Use a base de dados pública de **Kaggle** ou outro repositório de fácil acesso. Recomendo a base de dados "E-commerce Data" disponível no Kaggle:
- [E-commerce Data (Kaggle)](https://www.kaggle.com/olistbr/brazilian-ecommerce)
- Esta base contém informações de pedidos, clientes, vendedores e pagamentos de um marketplace brasileiro.

---

#### **2. Modelagem do Data Warehouse**
- **Modelo Star Schema (Esquema Estrela):**
  - **Tabela Fato:** Vendas
    - Colunas: ID da Venda, Data da Venda, ID do Cliente, ID do Produto, ID do Vendedor, Quantidade Vendida, Valor Total, Frete.
  - **Dimensões:**
    - Dimensão Data: Detalhes da data (ano, mês, dia, trimestre, etc.).
    - Dimensão Cliente: ID do Cliente, Nome, Cidade, Estado, etc.
    - Dimensão Produto: ID do Produto, Nome, Categoria, etc.
    - Dimensão Vendedor: ID do Vendedor, Nome, Região, etc.

---

#### **3. Processos ETL**
- **Extract:** Baixe e carregue os dados brutos.
- **Transform:** 
  - Limpeza de dados: Remova inconsistências e preencha valores ausentes.
  - Enriquecimento: Crie campos derivados, como faixa etária dos clientes ou categorias consolidadas de produtos.
- **Load:** Carregue os dados transformados no Data Warehouse.

---

#### **4. Consultas e KPIs**
Implemente as seguintes análises:
1. **Vendas por Região e Produto:** Qual região mais contribui para a receita? Quais são os produtos mais vendidos?
2. **Churn de Clientes:** Qual a porcentagem de clientes que não fizeram compras nos últimos meses?
3. **Tempo de Entrega:** Média de tempo de entrega por categoria de produto.
4. **Margem de Lucro:** Qual a margem de lucro por produto, categoria ou região?
5. **Vendas sazonais:** Identifique períodos de maior volume de vendas.

---

#### **5. Ferramentas e Tecnologias**
- **Base de Dados:** PostgreSQL
- **ETL:** Scripts Python com pandas.
- **Visualização:** Streamlit, lib do python
- **Consultas SQL:** Para consolidar dados e responder às perguntas de negócio.

---

#### **6. Entregáveis**
1. Esquema do Data Warehouse documentado.
2. Script do pipeline ETL.
3. Consultas SQL para análises específicas.
4. Dashboard com KPIs relevantes.

---

**Desafio adicional:** 
- Adicione dados complementares, como populações regionais ou tendências de busca do Google Trends, para análises mais ricas.
- Utilize particionamento e indexação para otimizar as consultas.

Este projeto irá testar suas habilidades de modelagem, ETL, otimização de consultas SQL e construção de relatórios analíticos! Se precisar de ajuda em alguma etapa, é só avisar!


