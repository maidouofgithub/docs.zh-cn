---
title: 在 Linux CentOS 8 上安装 .NET Core - 包管理器 - .NET Core
description: 使用包管理器在 CentOS 8 上安装 .NET Core SDK 和运行时。
author: thraka
ms.author: adegeo
ms.date: 05/01/2020
ms.openlocfilehash: b4cf5975e18aa8dfa8649c0d038caf38d648ad86
ms.sourcegitcommit: 7370aa8203b6036cea1520021b5511d0fd994574
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/02/2020
ms.locfileid: "82728503"
---
# <a name="centos-8-package-manager---install-net-core"></a><span data-ttu-id="7fbbf-103">CentOS 8 包管理器 - 安装 .NET Core</span><span class="sxs-lookup"><span data-stu-id="7fbbf-103">CentOS 8 Package Manager - Install .NET Core</span></span>

[!INCLUDE [package-manager-switcher](includes/package-manager-switcher.md)]

<span data-ttu-id="7fbbf-104">本文介绍如何使用包管理器在 CentOS 8 上安装 .NET Core。</span><span class="sxs-lookup"><span data-stu-id="7fbbf-104">This article describes how to use a package manager to install .NET Core on CentOS 8.</span></span>

[!INCLUDE [package-manager-intro-sdk-vs-runtime](includes/package-manager-intro-sdk-vs-runtime.md)]

## <a name="install-the-net-core-sdk"></a><span data-ttu-id="7fbbf-105">安装 .NET Core SDK</span><span class="sxs-lookup"><span data-stu-id="7fbbf-105">Install the .NET Core SDK</span></span>

<span data-ttu-id="7fbbf-106">在终端中，运行以下命令。</span><span class="sxs-lookup"><span data-stu-id="7fbbf-106">In your terminal, run the following command.</span></span>

```bash
sudo dnf install dotnet-sdk-3.1
```

## <a name="install-the-aspnet-core-runtime"></a><span data-ttu-id="7fbbf-107">安装 ASP.NET Core 运行时</span><span class="sxs-lookup"><span data-stu-id="7fbbf-107">Install the ASP.NET Core Runtime</span></span>

<span data-ttu-id="7fbbf-108">在终端中，运行以下命令。</span><span class="sxs-lookup"><span data-stu-id="7fbbf-108">In your terminal, run the following command.</span></span>

```bash
sudo dnf install aspnetcore-runtime-3.1
```

## <a name="install-the-net-core-runtime"></a><span data-ttu-id="7fbbf-109">安装 .NET Core 运行时</span><span class="sxs-lookup"><span data-stu-id="7fbbf-109">Install the .NET Core Runtime</span></span>

<span data-ttu-id="7fbbf-110">在终端中，运行以下命令。</span><span class="sxs-lookup"><span data-stu-id="7fbbf-110">In your terminal, run the following command.</span></span>

```bash
sudo dnf install dotnet-runtime-3.1
```

## <a name="how-to-install-other-versions"></a><span data-ttu-id="7fbbf-111">如何安装其他版本</span><span class="sxs-lookup"><span data-stu-id="7fbbf-111">How to install other versions</span></span>

[!INCLUDE [package-manager-switcher](./includes/package-manager-heading-hack-pkgname.md)]