---
title: gRPC for .NET supported platforms
author: jamesnk
description: Learn about the supported platforms for gRPC on .NET.
monikerRange: '>= aspnetcore-3.0'
ms.author: jamesnk
ms.date: 01/22/2021
no-loc: [appsettings.json, "ASP.NET Core Identity", cookie, Cookie, Blazor, "Blazor Server", "Blazor WebAssembly", "Identity", "Let's Encrypt", Razor, SignalR]
uid: grpc/supported-platforms
---
# gRPC for .NET supported platforms

By [James Newton-King](https://twitter.com/jamesnk)

## Device requirements

gRPC for .NET supports any device that .NET Core supports.

> [!div class="checklist"]
>
> * Windows
> * Linux
> * macOS&dagger;

&dagger;ASP.NET Core websites on macOS doesn't support HTTPS. gRPC clients on macOS can still use HTTPS when calling remote services.

## ASP.NET Core server requirements

gRPC services can be hosted on all built-in ASP.NET Core servers.

> [!div class="checklist"]
>
> * Kestrel
> * TestServer
> * IIS&dagger;
> * HttpSys&dagger;

&dagger;IIS and HttpSys require .NET 5 and Windows XXXX or later

## .NET version requirements

gRPC for .NET supports .NET Core 3 and .NET 5 or later.

> [!div class="checklist"]
>
> * .NET 5 or later
> * .NET Core 3

gRPC for .NET doesn't support running on .NET Framework and Xamarin/Mono. [gRPC C# core-library](https://grpc.io/docs/languages/csharp/quickstart/) is a third party library that supports .NET Framework and Xamarin/Mono. This library is not supported by Microsoft.

## Azure services

> [!div class="checklist"]
>
> * [Azure Kubernetes Service (AKS)](https://azure.microsoft.com/services/kubernetes-service/)
> * [Azure App Service](https://azure.microsoft.com/services/app-service/)&dagger;

&dagger;Azure App Service doesn't support hosting gRPC over HTTP/2.  gRPC-Web is the recommended alternative, it doesn't require HTTP/2 and supports most of gRPC's features.

## Additional resources

* [gRPC C# core-library](https://grpc.io/docs/languages/csharp/quickstart/)
