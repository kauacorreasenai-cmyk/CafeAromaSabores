# ☕ CafeAromaESabor - Gestão de Estoque

Sistema desenvolvido para o controle de almoxarifado de uma cafeteria, focado na rastreabilidade de lotes, gestão de estoque mínimo e controle de movimentações.

---

## 🚀 Funcionalidades Implementadas

### 1. Gestão Completa (CRUD)
O sistema permite o gerenciamento total das entidades principais:
* **Produtos:** Cadastro de nome, descrição, lote e data de validade.
* **Movimentações:** Registro de entradas e saídas com histórico detalhado.
* **Usuários:** Controle de quem opera o sistema.

### 2. Segurança e Acesso
* **Spring Security:** Implementação de camadas de segurança para proteger as rotas.
* **Autenticação:** Sistema de login e logout funcional.
* **Níveis de Acesso:** Proteção de dados sensíveis contra acessos não autorizados.

### 3. Regras de Negócio
* **Estoque Mínimo:** Monitoramento de quantidades para evitar rupturas no estoque.
* **Rastreabilidade:** Cada movimentação é vinculada automaticamente a um produto, um usuário e um carimbo de data/hora.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Java 21
* **Framework:** Spring Boot 3
* **Persistência:** Spring Data JPA
* **Banco de Dados:** MySQL 8.0
* **Interface:** Thymeleaf (HTML/CSS)
* **Segurança:** Spring Security

---

## 📊 Modelagem de Dados
A estrutura do banco de dados foi gerada e validada através de **Engenharia Reversa** utilizando o MySQL Workbench, garantindo que os relacionamentos `@ManyToOne` entre Movimentação, Produto e Usuário fossem criados corretamente.

---

## 📋 Como Executar o Projeto

1. Clone o repositório: `git clone https://github.com/kauacorreasenai-cmyk/CafeAromaSabores.git`
2. Configure o banco de dados MySQL com o nome `cafearomasabor`.
3. Ajuste as credenciais no arquivo `src/main/resources/application.properties`.
4. Execute a classe `CafeAromaSaboresApplication`.