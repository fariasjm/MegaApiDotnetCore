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

<p align="center">
  Esta API em .NET Core foi desenvolvida para fornecer dados em formato JSON sobre os chefes da série de jogos Mega Man.
  Ela funciona como um serviço backend construído com .NET Core 3.1, oferecendo acesso estruturado e confiável aos dados dos robôs mestres de diversos jogos da franquia.
  <br />
</p>

<p align="center">
  Principais Funcionalidades:
    Entity Framework Core para interações com o banco de dados de forma eficiente e escalável.
    Design RESTful para fácil consumo por aplicações frontend, clientes mobile ou outros serviços.
    Respostas em JSON formatadas para facilitar a integração.
    Desenvolvida com tecnologias modernas do .NET e boas práticas para garantir desempenho e manutenibilidade.

  Casos de Uso:
    Ideal para fãs, desenvolvedores ou criadores de conteúdo que desejam integrar dados dos chefes de Mega Man em aplicações, dashboards ou ferramentas relacionadas a jogos.
  <br />
</p>

<p align="center">
  <br />
  <img src="./_docs/assets/carbon.png" />
</p>

## API Endpoints

<table align="center">
  <tr>
    <th>Method</th>
    <th>Endpoint</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>GET</td>
    <td>/api/v1/robots</td>
    <td>Returns a list of all robots</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/api/v1/robots/{id}</td>
    <td>Returns details of a specific robot by ID</td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/api/v1/robots</td>
    <td>Endpoint to create a new robot entry</td>
  </tr>
</table>

## Techniques Used

<p align="center">
  - <b>Entity Framework Core:</b> ORM for data management.<br />
  - <b>RESTful API Design:</b> Ensures clear and effective communication
  endpoints.<br />
  - <b>Dependency Injection:</b> Used throughout to promote loose coupling and
  enhanced testability.<br />
</p>

## Dependencies

<table align="center">
  <tr>
    <th>Package</th>
    <th>Version</th>
    <th>Link</th>
  </tr>
  <tr>
    <td>Microsoft.EntityFrameworkCore</td>
    <td>3.1.8</td>
    <td>
      <a
        href="https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/3.1.8"
        >NuGet</a
      >
    </td>
  </tr>
  <tr>
    <td>Microsoft.EntityFrameworkCore.Design</td>
    <td>3.1.8</td>
    <td>
      <a
        href="https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design/3.1.8"
        >NuGet</a
      >
    </td>
  </tr>
  <tr>
    <td>Microsoft.EntityFrameworkCore.SqlServer</td>
    <td>3.1.8</td>
    <td>
      <a
        href="https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/3.1.8"
        >NuGet</a
      >
    </td>
  </tr>
  <tr>
    <td>Newtonsoft.Json</td>
    <td>12.0.2</td>
    <td>
      <a href="https://www.nuget.org/packages/Newtonsoft.Json/12.0.2">NuGet</a>
    </td>
  </tr>
</table>

## :gear: Arch

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

## License This software is licensed under the terms of the [MIT]

⌨️ FelipeAguiar -
[Github](https://github.com/felipeAguiarCode)
