<h1 align="center">
  <br />
  <img
    src="./_docs/assets/icon.png"
    alt="Mega Man Robots API"
    width="150"
  />
  <br />
  <b>Mega Man Robots API</b>
  <br />
  <sub
    ><sup><b>(MEGA-MAN-ROBOTS)</b></sup></sub
  >
  <br />
  <a
    href="https://github.com/felipeAguiarCode/MegaApiDotnetCore/actions/workflows/build.yml"
  >
    <img
      src="https://github.com/felipeAguiarCode/MegaApiDotnetCore/actions/workflows/build.yml/badge.svg"
      alt=""
    />
  </a>
  <a href="https://github.com/felipeAguiarCode/MegaApiDotnetCore/releases/latest">
    <img
      src="https://img.shields.io/github/v/release/felipeAguiarCode/MegaApiDotnetCore"
      alt="Latest Release"
    />
  </a>
</h1>

  Esta API em .NET Core foi desenvolvida para fornecer dados em formato JSON sobre os chefes da série de jogos Mega Man.
  Ela funciona como um serviço backend construído com .NET Core 3.1, oferecendo acesso estruturado e confiável aos dados dos robôs mestres de diversos jogos da franquia.
 

### Principais Funcionalidades:
  - Entity Framework Core para interações com o banco de dados de forma eficiente e escalável.
  - Design RESTful para fácil consumo por aplicações frontend, clientes mobile ou outros serviços.
  - Respostas em JSON formatadas para facilitar a integração.
  - Desenvolvida com tecnologias modernas do .NET e boas práticas para garantir desempenho e manutenibilidade.

### Casos de Uso:
  Ideal para fãs, desenvolvedores ou criadores de conteúdo que desejam integrar dados dos chefes de Mega Man
em aplicações, dashboards ou ferramentas relacionadas a jogos.
 
<p align="center">
  <br />
  <img src="./_docs/assets/carbon.png" />
</p>

### API Endpoints

<table align="center">
  <tr>
    <th>Method</th>
    <th>Endpoint</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>GET</td>
    <td>/api/v1/robots</td>
    <td>Retorna uma lista de todos os robôs (chefes) disponíveis no banco de dados</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/api/v1/robots/{id}</td>
    <td>Retorna informações detalhadas sobre um robô (chefe) específico com base no seu ID único</td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/api/v1/robots</td>
    <td>Cria uma nova entrada de robô (chefe) no banco de dados</td>
  </tr>
</table>

### Técnicas Utilizadas
  - Entity Framework Core: ORM para gerenciamento de dados de forma eficiente e estruturada.
  - Design de API RESTful: Garante endpoints de comunicação claros, consistentes e eficazes.
  - Injeção de Dependência: Utilizada em toda a aplicação para promover baixo acoplamento, modularidade e maior facilidade de testes.

### Dependências

O projeto depende dos seguintes pacotes NuGet e tecnologias principais:

  - Microsoft.EntityFrameworkCore – ORM (mapeador objeto-relacional) para acesso ao banco de dados
  - Microsoft.AspNetCore.Mvc – Componentes principais para construção de APIs web
  - Microsoft.Extensions.DependencyInjection – Suporte nativo à injeção de dependência
  - Swashbuckle.AspNetCore – Geração de documentação Swagger/OpenAPI
  - Newtonsoft.Json (opcional) – Serialização JSON avançada (se necessário)
  - Microsoft.EntityFrameworkCore.SqlServer ou Sqlite – Provedor de banco de dados (dependendo da configuração)

### Arquitetura
O projeto segue uma arquitetura limpa e modular, visando manutenibilidade e escalabilidade:

```🌐
src
├── 📂 Controllers      [Routes for endpoints]
├── 📂 Models           [Database models]
├── 📂 Services         [Business rules]
├── 📂 Middlewares      [Intermediate functions between the HTTP request and the final server response]
├── 📂 Database         [Structures related to the database]
│   ├── 📂 DTOs             [Input Models and View Models (Data Transfer Objects)]
│   ├── 📂 EntityFramework  [Files related to the ORM Entity Framework]
│   │     ├── 📂 Context         [Entity context settings]
│   │     ├── 📂 Migrations      [Migrations for database updates]
│   ├── 📂 Repositories     [Repository pattern]
```

### Licença
Este software está licenciado sob os termos da Licença MIT.

Você é livre para usar, modificar e distribuir, desde que mantenha a devida atribuição e inclua a licença original.


⌨️ FelipeAguiar -
[Github](https://github.com/felipeAguiarCode)
