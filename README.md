# LOJINHA 

**Estrutura da Aplicação - Parte 1**

---

**Requisitos:**

1. **ASP.NET Core 6.0:** Framework principal para desenvolvimento web em C#.
2. **Entity Framework Core 6.0:** ORM para manipulação de banco de dados.
3. **Flunt.BR 3.0:** Para validações fluentes.
4. **RabbitMQ:** Sistema de mensagens para filas.
5. **Redis:** Banco de dados em memória para caching.
6. **Microsoft.Extensions.Caching.StackExchangeRedis 7.0:** Pacote para integração com Redis para caching.
7. **Swashbuckle.AspNetCore 7.0:** Biblioteca para geração de documentação da API (Swagger).
8. **Microsoft.EntityFrameworkCore.SqlServer 7.0:** Driver para SQL Server no Entity Framework Core.
9. **Microsoft.AspNetCore.Mvc.NewtonsoftJson 7.0:** Suporte ao JSON.NET no ASP.NET Core.

---

**Instalação de Recursos:**

1. **ASP.NET Core 6.0:**
   - [Download e instruções](https://dotnet.microsoft.com/download/dotnet/6.0)

2. **Entity Framework Core 6.0:**
   ```bash
   dotnet add package Microsoft.EntityFrameworkCore.SqlServer --version 6.0.0
   dotnet add package Microsoft.EntityFrameworkCore.Tools --version 6.0.0
   ```

3. **Flunt.BR 3.0:**
   ```bash
   dotnet add package Flunt.Br --version 3.0.0
   ```

4. **RabbitMQ:**
   - [Download e instruções](https://www.rabbitmq.com/download.html)

5. **Redis:**
   - [Download e instruções](https://redis.io/download)

6. **Microsoft.Extensions.Caching.StackExchangeRedis 7.0:**
   ```bash
   dotnet add package Microsoft.Extensions.Caching.StackExchangeRedis --version 7.0.0
   ```

7. **Swashbuckle.AspNetCore 7.0:**
   ```bash
   dotnet add package Swashbuckle.AspNetCore --version 7.0.0
   ```

8. **Microsoft.EntityFrameworkCore.SqlServer 7.0:**
   ```bash
   dotnet add package Microsoft.EntityFrameworkCore.SqlServer --version 7.0.0
   ```

9. **Microsoft.AspNetCore.Mvc.NewtonsoftJson 7.0:**
   ```bash
   dotnet add package Microsoft.AspNetCore.Mvc.NewtonsoftJson --version 7.0.0
   ```

---

**Preparação de Ambientes:**

1. **Configuração do Banco de Dados:**
   - Configure sua conexão SQL Server no arquivo `appsettings.json`.
   - Execute as migrações: `dotnet ef database update`.

2. **Configuração do Redis:**
   - Configure a conexão com o Redis no arquivo `appsettings.json`.

3. **Configuração do RabbitMQ:**
   - Inicie o servidor RabbitMQ.
   - Configure a conexão com o RabbitMQ no arquivo `appsettings.json`.

4. **Configuração do Swagger (Opcional):**
   - Configure o Swagger no arquivo `Startup.cs`.

---

**Referências:**

1. [ASP.NET Core Documentation](https://docs.microsoft.com/en-us/aspnet/core)
2. [Entity Framework Core Documentation](https://docs.microsoft.com/en-us/ef/core/)
3. [Flunt.BR Documentation](https://github.com/andrebaltieri/Flunt)
4. [RabbitMQ Documentation](https://www.rabbitmq.com/documentation.html)
5. [Redis Documentation](https://redis.io/documentation)
6. [Swashbuckle.AspNetCore Documentation](https://github.com/domaindrivendev/Swashbuckle.AspNetCore)
7. [Microsoft.Extensions.Caching.StackExchangeRedis Documentation](https://docs.microsoft.com/en-us/aspnet/core/performance/caching/distributed?view=aspnetcore-6.0#stack-exchange-redis-cache)
8. [Microsoft.EntityFrameworkCore.SqlServer Documentation](https://docs.microsoft.com/en-us/ef/core/providers/sql-server/?tabs=dotnet-core-cli)
9. [Microsoft.AspNetCore.Mvc.NewtonsoftJson Documentation](https://docs.microsoft.com/en-us/aspnet/core/web-api/advanced/formatting?view=aspnetcore-6.0#use-newtonsoftjson)

---

Essa estrutura fornece as bases necessárias para desenvolver uma aplicação utilizando ASP.NET Core 6.0 com as tecnologias mencionadas. Na Parte 2, iremos desenvolver os modelos, repositórios, queries, comandos e controllers para as entidades sugeridas.
