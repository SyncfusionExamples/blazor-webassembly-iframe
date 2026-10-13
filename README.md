# Blazor WebAssembly iFrame Sample

## Overview

This sample demonstrates how to embed an external website inside an HTML iframe within a Blazor WebAssembly application. The application uses the root page of a .NET 8 Blazor WebAssembly project to render a standard HTML `<iframe>` element that loads an external URL directly within the application interface.

The sample provides a simple reference implementation for displaying external web content such as documentation sites, dashboards, reports, portals, or other web-based resources inside a Blazor application. It focuses on native iframe integration without requiring additional JavaScript frameworks, custom hosting mechanisms, or third-party components.

## Key Features

- Uses the Blazor routing directive `@page "/"` to make the iframe page the application's default route.
- Renders a native HTML `<iframe>` element directly within the Blazor page.
- Embeds an external website using the iframe `src` attribute.
- Configures iframe dimensions through the `width="560"` and `height="315"` attributes.
- Removes the default iframe border using the `frameborder="0"` attribute.
- Enables fullscreen viewing support with the `allowfullscreen` attribute.
- Demonstrates a simple approach for displaying external web content within a Blazor WebAssembly application.
- Provides a minimal implementation that can be customized to load different external URLs inside the iframe.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download the repository.
2. Open the following solution file:

   `BlazorWebAssembly_NET8/BlazorWebAssembly_NET8.sln`

3. Restore all NuGet packages.
4. Build the solution.
5. Run the application using `Ctrl+F5`.

**Visual Studio Code**

1. Clone or download the repository.
2. Open the repository folder in Visual Studio Code.
3. Open a terminal and navigate to the project directory:

```bash
cd BlazorWebAssembly_NET8
```

4. Restore project dependencies:

```bash
dotnet restore
```

5. Run the application:

```bash
dotnet run
```

6. Open the local application URL displayed in the terminal after the project starts.

## Project Structure

`BlazorWebAssembly_NET8/Pages/Home.razor` - Defines the root page and renders an HTML iframe that loads content from `https://blazor.net`.

`BlazorWebAssembly_NET8/App.razor` - Configures the application's routing and page rendering pipeline.

`BlazorWebAssembly_NET8/Program.cs` - Initializes the Blazor WebAssembly host and configures application services.

`BlazorWebAssembly_NET8/_Imports.razor` - Contains shared Razor directives and namespace imports used throughout the application.

`BlazorWebAssembly_NET8/BlazorWebAssembly_NET8.csproj` - Project definition file that specifies the .NET target framework and project dependencies.

`BlazorWebAssembly_NET8/BlazorWebAssembly_NET8.sln` - Visual Studio solution file for the sample application.

`BlazorWebAssembly_NET8/wwwroot/index.html` - Client-side host page that bootstraps the Blazor WebAssembly application.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Review the official Blazor WebAssembly documentation: https://blazor.syncfusion.com/documentation/getting-started/blazor-webassembly-app

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.