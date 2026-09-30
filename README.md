# site-um-blazor

Projeto da disciplina de **Desenvolvimento Web** (Usabilidade, Dev. Web, Mobile e Jogos) - Anima Educação.
Professor: Daniel Henrique Matos de Paiva.

Lista de exercícios para praticar os conceitos básicos de Blazor: roteamento com `@page`, lógica em C# com `@code` e eventos com `@onclick`.

## Tecnologias

- .NET 10
- Blazor Web App (interatividade no servidor)
- C# / Razor

## Exercícios

| Exercício | Rota         | Arquivo                              | Foco                            |
|-----------|--------------|--------------------------------------|---------------------------------|
| 1         | `/sobre`     | `Components/Pages/Sobre.razor`       | Roteamento com `@page`          |
| 2         | `/contador`  | `Components/Pages/Contador.razor`    | `@code` e `@onclick`            |
| 3         | `/mensagem`  | `Components/Pages/Mensagem.razor`    | Estado booleano e `@if`         |
| 4         | `/placar`    | `Components/Pages/Placar.razor`      | Vários eventos no mesmo estado  |

### O que cada página faz

- **Sobre:** mostra o nome completo do aluno e uma breve descrição do curso.
- **Contador:** exibe "Número de cliques: X" e um botão que soma 1 a cada clique.
- **Mensagem:** um botão alterna entre "Exibir Mensagem" e "Ocultar Mensagem", mostrando ou escondendo o texto de boas-vindas.
- **Placar:** botões para somar 1, subtrair 1 e zerar os pontos. O placar nunca fica negativo.

## Estrutura do projeto

```
SiteUmBlazor/
├── Components/
│   ├── Layout/          # MainLayout e menu de navegação
│   ├── Pages/           # Páginas dos exercícios
│   ├── App.razor
│   ├── Routes.razor
│   └── _Imports.razor
├── Properties/
│   └── launchSettings.json
├── wwwroot/
│   └── app.css
├── Program.cs
└── SiteUmBlazor.csproj
```

## Como rodar

Pré-requisito: [SDK do .NET 10](https://dotnet.microsoft.com/download) instalado.

```bash
git clone https://github.com/SEU-USUARIO/site-um-blazor.git
cd site-um-blazor
dotnet watch
```

Depois acesse no navegador:

- http://localhost:5080
- http://localhost:5080/sobre
- http://localhost:5080/contador
- http://localhost:5080/mensagem
- http://localhost:5080/placar

Também é possível rodar pelo Visual Studio com **F5**.
