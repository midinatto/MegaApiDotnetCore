<h1>
    <img src="https://i.imgur.com/G6Mleco.png"> Megaman API
</h1>

<p align="center">
    <i>Uma API RESTful para listar dados dos bosses de Megaman</i><br />
    <br />
    <img src="https://vignette.wikia.nocookie.net/megaman/images/2/22/Cutman.png">
</p>

## 🚀 Início Rápido

### Pré-requisitos

Antes de começar, certifique-se de ter instalado:
- [.NET Core 3.1 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/3.1)
- [SQL Server](https://www.microsoft.com/pt-br/sql-server/sql-server-downloads) (se for utilizar o banco de dados local)

### Instalação

1. Clone o repositório:
   ```sh
   git clone https://github.com/seu-usuario/megaman-api.git
   cd megaman-api
   ```

2. Restaure as dependências:
   ```sh
   dotnet restore
   ```

3. Configure o banco de dados (opcional, se estiver usando Entity Framework):
   ```sh
   dotnet ef database update
   ```

4. Execute a API:
   ```sh
   dotnet run
   ```

A API estará disponível por padrão em `http://localhost:5000/api/v1/robots`.

## Uso

Para rodar esta API, é necessário ter o [.NET Core 3.1 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/3.1) instalado.

Após clonar o repositório, você pode rodar a API utilizando o seguinte comando:

```sh
  dotnet run
```

A API estará disponível por padrão em `http://localhost:5000/api/v1/robots`.

## Endpoints

- **GET /api/v1/robots** → Retorna todos os bosses disponíveis.
- **GET /api/v1/robots/{id}** → Retorna um boss específico pelo ID.
- **POST /api/v1/robots** → Adiciona um novo boss (ainda não implementado).

## Estrutura do Projeto

```
MegamanApi
├── .vs
├── .vscode
├── bin
├── Controllers
│   └── RobotsController.cs
├── Database
├── middlewares
├── Models
│   └── Robot.cs
├── obj
├── Properties
│   └── launchSettings.json
├── Services
│   └── IRobotServices.cs
├── appsettings.Development.json
├── appsettings.json
├── global.json
├── MegamanApi.csproj
├── MegamanApi.sln
├── Program.cs
└── Startup.cs
```

## Dependências

| Pacote | Versão | Descrição |
|--------|--------|-----------|
| [Microsoft.EntityFrameworkCore](https://docs.microsoft.com/en-us/ef/core/) | 3.1.8 | Biblioteca de acesso a dados para o Entity Framework Core. |
| [Microsoft.EntityFrameworkCore.Design](https://docs.microsoft.com/en-us/ef/core/) | 3.1.8 | Ferramentas de design para o Entity Framework Core. |
| [Microsoft.EntityFrameworkCore.SqlServer](https://docs.microsoft.com/en-us/ef/core/providers/sql-server/?tabs=dotnet-core-cli) | 3.1.8 | Provedor do Entity Framework Core para SQL Server. |
| [Newtonsoft.Json](https://www.newtonsoft.com/json) | 12.0.2 | Biblioteca popular para serialização JSON no .NET. |

## Técnicas Utilizadas

A API é baseada na arquitetura MVC (Model-View-Controller):

- **Controllers**: Controladores responsáveis pelo roteamento e lógica das requisições HTTP.
- **Models**: Representações das entidades de domínio, como o modelo `Robot.cs`.
- **Services**: Camada de serviços para encapsular lógica de negócios, como `IRobotServices.cs`.
- **Database**: Responsável pela conexão e manipulação do banco de dados via Entity Framework Core.
- **Middlewares**: Componentes para interceptação de requisições HTTP (autenticação, logging, etc.).

## Contato

Se precisar de suporte ou quiser contribuir para o projeto, sinta-se à vontade para entrar em contato via [GitHub](#) ou [Discord](#).



## License This software is licensed under the terms of the [MIT]

⌨️ Mirella Dinatto-
[Github](https://github.com/midinatto)
