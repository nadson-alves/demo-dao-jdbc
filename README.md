Demo DAO JDBC

Projeto desenvolvido durante meus estudos de Java, com o objetivo de praticar a conexão entre aplicações Java e bancos de dados MySQL utilizando JDBC.

Tecnologias utilizadas

Java 26

JDBC (Java Database Connectivity)

MySQL

MySQL Connector/J

IntelliJ IDEA

Estrutura do projeto

demojdbc/
├── src/
│   ├── application/
│   │   └── Program.java
│   └── db/
│       ├── DB.java
│       ├── DbException.java
│       └── DbIntegrityException.java
├── .gitignore
└── README.md

Funcionalidades e conceitos praticados

Conexão com banco de dados MySQL através do JDBC.

Leitura de configurações utilizando Properties.

Gerenciamento de conexões com Connection.

Execução de comandos SQL com PreparedStatement.

Tratamento de exceções personalizadas.

Fechamento de recursos do banco de dados.

Configuração do banco de dados

Crie um banco de dados MySQL chamado coursejdbc.

Exemplo de criação da tabela:

CREATE TABLE department (
    Id INT NOT NULL AUTO_INCREMENT,
    Name VARCHAR(60) NOT NULL,
    PRIMARY KEY (Id)
);

Adicione os registros:

INSERT INTO department (Name) VALUES
('Computers'),
('Electronics'),
('Fashion'),
('Books'),
('Management');

Configuração da conexão

Crie um arquivo chamado db.properties na raiz do projeto:

user=root
password=sua_senha
dburl=jdbc:mysql://localhost:3306/coursejdbc
useSSL=false

Substitua sua_senha pela senha do seu MySQL.

Importante: o arquivo db.properties não é enviado ao GitHub, pois contém informações de acesso ao banco de dados.

Objetivo

Este projeto faz parte da minha jornada de aprendizado em Java, aprofundando conhecimentos em persistência de dados, JDBC e integração com bancos de dados relacionais.
