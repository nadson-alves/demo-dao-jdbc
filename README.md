Demo DAO JDBC

Projeto desenvolvido em Java com o objetivo de praticar a integração com banco de dados MySQL utilizando JDBC e aplicar o padrão de arquitetura DAO (Data Access Object).

A aplicação permite realizar operações de consulta, inserção, atualização e exclusão de vendedores, além de trabalhar com relacionamentos entre vendedores e departamentos.

Tecnologias utilizadas

Java 26

JDBC (Java Database Connectivity)

MySQL

MySQL Connector/J

IntelliJ IDEA

Git e GitHub

Funcionalidades

Conexão com banco de dados MySQL utilizando JDBC.

Implementação do padrão DAO.

Separação entre interfaces e implementações JDBC.

Utilização da DaoFactory para criação dos objetos DAO.

Busca de vendedores por ID (findById).

Busca de vendedores por departamento (findByDepartment).

Consulta de todos os vendedores (findAll).

Cadastro de vendedores (insert).

Atualização de vendedores (update).

Exclusão de vendedores (deleteById).

Relacionamento entre vendedores e departamentos.

Tratamento de exceções personalizadas.

Gerenciamento de conexões e recursos JDBC.

Banco de dados

O projeto utiliza o MySQL com um banco de dados chamado coursejdbc.

São utilizadas duas tabelas principais:

Department

Id

Name

Seller

Id

Name

Email

BirthDate

BaseSalary

DepartmentId

A tabela Seller possui uma chave estrangeira (DepartmentId) que estabelece o relacionamento com a tabela Department.

Configuração

Para executar o projeto, é necessário:

Ter o Java JDK instalado.

Ter o MySQL instalado e em execução.

Criar o banco de dados coursejdbc.

Criar as tabelas department e seller.

Adicionar o MySQL Connector/J às bibliotecas do projeto.

Configurar o arquivo db.properties com as credenciais do banco de dados.

Exemplo de configuração:

user=root
password=sua_senha
dburl=jdbc:mysql://localhost:3306/coursejdbc
useSSL=false

Importante: o arquivo db.properties não deve ser enviado ao GitHub, pois contém informações de acesso ao banco de dados.

Objetivo do projeto

Este projeto faz parte da minha jornada de aprendizado em desenvolvimento Java, com foco em programação orientada a objetos, persistência de dados, integração com bancos relacionais e organização de aplicações utilizando o padrão DAO.

O desenvolvimento permite aplicar na prática conceitos importantes para a construção de aplicações Java conectadas a bancos de dados.
