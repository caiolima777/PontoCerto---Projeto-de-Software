# 🏪 Ponto Certo 👨‍💻

> Sistema web desenvolvido para modernizar o gerenciamento de uma mercearia, oferecendo compras online, controle de pedidos, promoções e programa de fidelidade para clientes.

<table>
  <tr>
    <td width="800px">
      <div align="justify">
        O <b>Ponto Certo</b> é uma plataforma web desenvolvida com o objetivo de digitalizar e otimizar os processos de uma mercearia. O sistema permite que clientes realizem compras online, acompanhem pedidos, consultem promoções e participem de um programa de fidelidade baseado em pontos.
        <br><br>
        Além das funcionalidades voltadas aos clientes, a aplicação disponibiliza uma área administrativa para gerenciamento de produtos, promoções, pedidos, avisos e regras de pontuação, proporcionando maior controle e eficiência na administração do negócio.
      </div>
    </td>
    <td>
      <div align="center">
        <img src="https://cdn-icons-png.flaticon.com/512/3081/3081559.png" alt="Logo do Projeto" width="120px"/>
      </div>
    </td>
  </tr>
</table>

---

## 🚧 Status do Projeto

![Status](https://img.shields.io/badge/status-concluído-green?style=for-the-badge)
![React](https://img.shields.io/badge/Frontend-React-blue?style=for-the-badge)
![Spring Boot](https://img.shields.io/badge/Backend-SpringBoot-success?style=for-the-badge)
![MySQL](https://img.shields.io/badge/Banco-MySQL-orange?style=for-the-badge)
![Versão](https://img.shields.io/badge/Versão-1.0.0-blue?style=for-the-badge)

---

## 📚 Índice

* [Links Úteis](#-links-úteis)
* [Sobre o Projeto](#-sobre-o-projeto)
* [Problema Identificado](#-problema-identificado)
* [Objetivos](#-objetivos)
* [Regras de Negócio](#-regras-de-negócio)
* [Funcionalidades Principais](#-funcionalidades-principais)
* [Atores do Sistema](#-atores-do-sistema)
* [Casos de Uso](#-casos-de-uso)
* [Tecnologias Utilizadas](#-tecnologias-utilizadas)
* [Arquitetura](#-arquitetura)
* [Diagramas UML](#-diagramas-uml)
* [Estrutura de Pastas](#-estrutura-de-pastas)
* [Instalação e Execução](#️-instalação-e-execução)
* [API REST](#-api-rest)
* [Testes](#-testes)
* [Documentações Utilizadas](#-documentações-utilizadas)
* [Autor](#-autor)
* [Licença](#-licença)

---

## 🔗 Links Úteis

* 📖 **PlantUML:** https://plantuml.com/
* 📄 **Documentação do Projeto:** Docs/Documentacao-Ponto-Certo.pdf
* 🧩 **Diagramas UML:** Diagramas/

---

## 📝 Sobre o Projeto

O Ponto Certo é uma aplicação web desenvolvida para proporcionar uma experiência digital moderna aos clientes de uma mercearia. A plataforma permite a realização de compras online, acompanhamento de pedidos, consulta de promoções e participação em programas de fidelidade.

O sistema foi construído utilizando React no frontend e Spring Boot no backend, oferecendo uma arquitetura moderna, segura e escalável para atender tanto clientes quanto administradores.

---

## ❗ Problema Identificado

Muitas pequenas mercearias ainda realizam o gerenciamento de produtos, pedidos e relacionamento com clientes de forma manual ou utilizando sistemas limitados. Isso pode gerar dificuldades no controle de estoque, acompanhamento de pedidos, divulgação de promoções e fidelização dos consumidores.

O Ponto Certo foi proposto para centralizar essas operações em uma única plataforma, proporcionando maior organização, eficiência e praticidade para todos os envolvidos.

---

## 🎯 Objetivos

### Objetivo Geral

Desenvolver uma plataforma web para gerenciamento de uma mercearia, permitindo compras online, controle administrativo e programa de fidelidade para clientes.

### Objetivos Específicos

* Permitir cadastro e autenticação de usuários;
* Disponibilizar catálogo de produtos online;
* Gerenciar carrinho de compras;
* Registrar e acompanhar pedidos;
* Disponibilizar promoções e avisos;
* Implementar programa de fidelidade baseado em pontos;
* Permitir solicitação de resgates;
* Disponibilizar área administrativa para gerenciamento do sistema.

---

## 📌 Regras de Negócio

| ID    | Regra de Negócio                                                           |
| ----- | -------------------------------------------------------------------------- |
| RN-01 | Apenas usuários cadastrados podem realizar compras.                        |
| RN-02 | Todo pedido deve estar associado a um cliente válido.                      |
| RN-03 | O cliente acumula pontos após a conclusão de compras.                      |
| RN-04 | Apenas clientes com saldo suficiente podem solicitar resgates.             |
| RN-05 | Solicitações de resgate devem passar por aprovação administrativa.         |
| RN-06 | Administradores podem cadastrar, editar e remover produtos.                |
| RN-07 | Promoções podem ser associadas a produtos específicos.                     |
| RN-08 | Avisos podem ser publicados para todos os usuários do sistema.             |
| RN-09 | O acesso às funcionalidades administrativas exige perfil de administrador. |
| RN-10 | A autenticação é realizada utilizando tokens JWT.                          |

---

## ✨ Funcionalidades Principais

* 🔐 Autenticação de usuários
* 👤 Gerenciamento de perfil
* 📍 Cadastro de endereços
* 🛒 Carrinho de compras
* 📦 Gerenciamento de pedidos
* 🏷️ Promoções
* 📢 Avisos
* ⭐ Programa de fidelidade
* 🎁 Solicitação de resgates
* 👨‍💼 Painel administrativo
* 📊 Gerenciamento de produtos
* 👥 Gerenciamento de usuários
* 🔒 Controle de acesso com JWT

---

## 👥 Atores do Sistema

| Ator              | Descrição                                                                                     |
| ----------------- | --------------------------------------------------------------------------------------------- |
| Cliente           | Realiza compras, acompanha pedidos, consulta promoções e participa do programa de fidelidade. |
| Administrador     | Gerencia produtos, promoções, pedidos, avisos, usuários e regras de pontuação.                |
| Sistema de E-mail | Responsável pelo envio de mensagens de verificação e recuperação de senha.                    |

---

## 📍 Casos de Uso

| ID    | Caso de Uso                   | Ator Principal |
| ----- | ----------------------------- | -------------- |
| UC-01 | Realizar Cadastro             | Cliente        |
| UC-02 | Realizar Login                | Cliente        |
| UC-03 | Gerenciar Perfil              | Cliente        |
| UC-04 | Gerenciar Endereços           | Cliente        |
| UC-05 | Visualizar Produtos           | Cliente        |
| UC-06 | Gerenciar Carrinho            | Cliente        |
| UC-07 | Finalizar Pedido              | Cliente        |
| UC-08 | Consultar Pedidos             | Cliente        |
| UC-09 | Consultar Promoções           | Cliente        |
| UC-10 | Solicitar Resgate             | Cliente        |
| UC-11 | Gerenciar Produtos            | Administrador  |
| UC-12 | Gerenciar Promoções           | Administrador  |
| UC-13 | Gerenciar Pedidos             | Administrador  |
| UC-14 | Gerenciar Usuários            | Administrador  |
| UC-15 | Gerenciar Regras de Pontuação | Administrador  |

## 🛠 Tecnologias Utilizadas

### 💻 Front-end

* React
* Vite
* Bootstrap
* React Router
* Context API

### 🖥️ Back-end

* Java 21
* Spring Boot
* Spring Security
* Spring Data JPA
* Hibernate
* JWT

### 🗄️ Banco de Dados

* MySQL
* H2 Database (testes)

### ⚙️ Infraestrutura & DevOps

* Docker
* Docker Compose
* GitHub Actions

### 🧪 Qualidade e Testes

* JUnit
* Mockito
* Jacoco
* SonarQube
* OWASP Dependency Check
* Trivy

### 📐 Modelagem e Documentação

* PlantUML
* Markdown
* UML

---

## 🏗 Arquitetura

O sistema foi desenvolvido utilizando uma arquitetura em camadas, separando a aplicação em frontend, backend, segurança e persistência de dados.

### Visão Geral

```text
Cliente
   ↓
Frontend React
   ↓
API REST Spring Boot
   ↓
Spring Security + JWT
   ↓
Spring Data JPA / Hibernate
   ↓
Banco de Dados MySQL
```

Essa estrutura facilita a manutenção, escalabilidade e organização do projeto, além de proporcionar maior segurança no controle de acesso dos usuários.

---

## 📊 Diagramas UML

Os diagramas do sistema foram elaborados utilizando PlantUML e documentam os principais aspectos estruturais e comportamentais da aplicação.

| Diagrama                                  |
| ----------------------------------------- |
| Diagrama de Caso de Uso                   |
| Diagrama de Classes                       |
| Diagrama de Componentes                   |
| Diagrama de Implantação                   |
| Diagrama de Sequência – Login             |
| Diagrama de Sequência – Finalizar Pedido  |
| Diagrama de Sequência – Solicitar Resgate |
| Diagrama de Comunicação – Login           |
| Diagrama de Comunicação – Pedido          |
| Diagrama de Comunicação – Resgate         |
| Diagrama de Estado – Pedido               |
| Diagrama de Estado – Resgate              |
| Diagrama de Estado – Carrinho             |
| Diagrama de Estado – Usuário              |
| Modelo de Dados (DER)                     |

---

## 📁 Estrutura de Pastas

```text
PontoCerto/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── contexts/
│   │   ├── pages/
│   │   ├── services/
│   │   └── assets/
│   │
│   └── package.json
│
├── backend/
│   ├── src/
│   │   ├── controller/
│   │   ├── service/
│   │   ├── repository/
│   │   ├── model/
│   │   ├── dto/
│   │   ├── security/
│   │   └── config/
│   │
│   └── pom.xml
│
├── Docs/
├── Diagramas/
├── README.md
└── docker-compose.yml
```

---

## ▶️ Instalação e Execução

### Pré-requisitos

* Git
* Node.js
* npm
* Java 21
* Maven
* MySQL
* Docker (opcional)

### Clonar o repositório

```bash
git clone <url-do-repositorio>
```

```bash
cd PontoCerto
```

### Executar o Backend

```bash
cd backend
mvn spring-boot:run
```

A API ficará disponível em:

```text
http://localhost:8080
```

### Executar o Frontend

```bash
cd frontend
npm install
npm run dev
```

A aplicação ficará disponível em:

```text
http://localhost:5173
```

---

## 🔌 API REST

Principais recursos disponibilizados pela API:

### Autenticação

* Login
* Cadastro
* Recuperação de senha
* Verificação de conta

### Clientes

* Perfil
* Endereços
* Histórico de pedidos

### Produtos

* Consulta de produtos
* Promoções
* Gerenciamento administrativo

### Pedidos

* Carrinho
* Finalização de compra
* Consulta de pedidos

### Fidelidade

* Consulta de pontos
* Solicitação de resgates
* Gerenciamento de regras de pontuação

---

## 🧪 Testes

O projeto utiliza testes automatizados para validação das regras de negócio e dos principais serviços da aplicação.

| Tipo de Teste          | Objetivo                                |
| ---------------------- | --------------------------------------- |
| Testes Unitários       | Validar métodos isoladamente            |
| Testes de Serviço      | Verificar regras de negócio             |
| Testes de Segurança    | Validar autenticação e autorização      |
| Testes de Persistência | Verificar integração com banco de dados |
| Testes de API          | Validar endpoints REST                  |

Além disso, ferramentas como Jacoco, SonarQube e OWASP Dependency Check são utilizadas para análise de qualidade e segurança do código.

---

## 📚 Documentações Utilizadas

* PlantUML
* Spring Boot Documentation
* Spring Security Documentation
* React Documentation
* Hibernate Documentation
* MySQL Documentation
* Docker Documentation
* GitHub Actions Documentation

---

## 👤 Autor

| Nome      |
| --------- |
| Caio Lima |

---

## 🤝 Contribuição

Este projeto foi desenvolvido para fins acadêmicos como parte da disciplina Projeto de Software.

Contribuições externas não estão previstas para esta versão.

---

## 📄 Licença

Este projeto possui finalidade acadêmica.

Todos os direitos reservados ao autor.
