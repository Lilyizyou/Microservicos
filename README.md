![Bootcamp Java DIO](https://img.shields.io/badge/Bootcamp-DIO%20Java-blueviolet?style=for-the-badge&logo=java)
# 🛠️ Sistema de Gestão de Pedidos — Microserviços com Spring Boot & Spring Cloud

Este projeto é parte de um desafio técnico proposto pela NTT DATA Inc. e tem como objetivo desenvolver uma aplicação baseada em microserviços utilizando Spring Boot e Spring Cloud, aplicando conceitos modernos como Service Discovery, API Gateway, comunicação entre serviços e autenticação simplificada.

⚠️ **Status do Projeto**  
Este projeto ainda está em desenvolvimento e ainda foi finalizado.  
A estrutura principal foi iniciada, incluindo os microserviços e a arquitetura proposta, mas algumas funcionalidades ainda estão pendentes de implementação e testes. Pretendo continuar trabalhando nele para concluir todos os requisitos técnicos e aprimorar a solução.

---

## 📦 Arquitetura Proposta

- **Browser** → Interface de acesso
- **API Gateway** → Porta 8700–8799
- **Service Discovery (Eureka Server)**
- **Microserviço 1 — Catálogo de Produtos** → Porta 8100–8199
- **Microserviço 2 — Simulador de Pedidos** → Porta 8200–8299
- **Banco de Dados H2** → Persistência local para o catálogo

---

## 📋 Funcionalidades

### Microserviço 1 — Catálogo de Produtos
- Cadastro de produtos (nome, descrição, preço)
- Listagem e consulta de produtos
- Persistência via H2 Database

### Microserviço 2 — Simulador de Pedidos
- Consulta de produtos via Microserviço 1
- Simulação de criação de pedidos
- Sem persistência

---

## 🔐 Autenticação

- Autenticação simplificada via token fixo
- O token deve ser enviado no header:  
  `Authorization: Bearer <token>`
- Validação feita no API Gateway via filtro customizado

---

## 🚧 Progresso

- [x] Estrutura inicial dos microserviços
- [x] Configuração do Eureka Server
- [x] API Gateway com roteamento básico
- [ ] Implementação completa dos endpoints REST
- [ ] Autenticação via token
- [ ] Testes e documentação final

---

## 📚 Tecnologias Utilizadas

- Java 17
- Spring Boot
- Spring Cloud (Eureka, Gateway)
- Spring Security
- H2 Database

---

## 📌 Observações

Este projeto foi desenvolvido com foco em boas práticas REST, modularidade e escalabilidade.  
Ainda que não esteja finalizado, a base está sólida e pronta para evoluir.
