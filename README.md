# PIM Help Desk - Backend

![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=c-sharp&logoColor=white)
![MicrosoftSQLServer](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white)

---

## 📝 Sobre o Projeto

Este repositório contém o código-fonte do **backend** para o sistema de Help Desk, desenvolvido em **ASP.NET Core** como parte de um Projeto Integrado Multidisciplinar (PIM). A aplicação consiste em uma API RESTful responsável por todas as regras de negócio, gerenciamento de dados e autenticação da plataforma.

Esta API serve como a espinha dorsal para o [frontend em React](https://github.com/VictorMartelli/pim_help_desk_front), fornecendo os endpoints necessários para a manipulação de usuários, chamados e autenticação.

---

## ✨ Funcionalidades

- **API RESTful**: Arquitetura padronizada para comunicação com o cliente.
- **Autenticação e Autorização**: Sistema seguro baseado em JSON Web Tokens (JWT) para proteger os endpoints.
- **Gerenciamento de Dados**: Operações de CRUD (Create, Read, Update, Delete) para as entidades do sistema, como usuários e chamados.
- **Persistência de Dados**: Utilização do Entity Framework Core como ORM para mapeamento e comunicação com o banco de dados SQL Server.
- **Documentação da API**: Geração automática de documentação interativa com OpenAPI (Swagger/Scalar) para facilitar o teste e a integração.

---

## 🛠️ Tecnologias Utilizadas

A tabela abaixo lista as principais tecnologias e pacotes que compõem o projeto:

| Tecnologia/Pacote | Versão/Descrição |
| ------------------- | ------------------------------------------------------------ |
| **.NET** | `9.0` - Framework principal para a construção da aplicação. |
| **ASP.NET Core** | Plataforma para criação de APIs web de alta performance. |
| **Entity Framework Core** | `9.0.3` - ORM para interação com o banco de dados. |
| **SQL Server** | Provider do EF Core para o banco de dados Microsoft SQL Server. |
| **JWT Bearer Authentication** | `8.6.1` - Middleware para autenticação baseada em tokens JWT. |
| **OpenAPI (Swagger)** | `9.0.3` - Geração de documentação para a API. |
| **Scalar.AspNetCore** | `2.1.0` - Interface alternativa para a documentação da API. |

---

## 🚀 Como Executar o Projeto

Para executar o projeto localmente, você precisará do [.NET SDK](https://dotnet.microsoft.com/download) instalado. Siga os passos abaixo:

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/VictorMartelli/pim_help_desk.git
   ```

2. **Acesse a pasta do projeto:**
   ```bash
   cd pim_help_desk/PIM_Help_Desk
   ```

3. **Configure a Connection String:**
   - Abra o arquivo `appsettings.json`.
   - Modifique a `DefaultConnection` para apontar para a sua instância do SQL Server.

4. **Aplique as Migrations:**
   - Execute o comando abaixo para criar e atualizar as tabelas no banco de dados.
   ```bash
   dotnet ef database update
   ```

5. **Execute a aplicação:**
   ```bash
   dotnet run
   ```

A API estará em execução e acessível (por padrão, em `https://localhost:7123`). A documentação interativa da API pode ser acessada através do endpoint `/swagger`.

---

## 📄 Licença

Este projeto está sob a licença MIT. Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 👨‍💻 Autor

Desenvolvido por Victor Martelli e alunos do 4° Semestre do CST em Análise e Desenvolvimento de Sistemas da Universidade Paulista - Unip (Araraquara)

[LinkedIn:] (www.linkedin.com/in/victormartelli)
