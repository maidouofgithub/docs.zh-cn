---
title: 程序集和 DLL 的名称
ms.date: 10/22/2008
ms.technology: dotnet-standard
helpviewer_keywords:
- names [.NET Framework], DLLs
- names [.NET Framework], assemblies
- assemblies [.NET Framework], names
- DLLs, names
ms.assetid: e800b610-31b4-4949-9c14-cb60e9f254be
ms.openlocfilehash: 138ae8154b0d10fb813f0c98ceb7c58a2471b780
ms.sourcegitcommit: 33deec3e814238fb18a49b2a7e89278e27888291
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "84291950"
---
# <a name="names-of-assemblies-and-dlls"></a>程序集和 DLL 的名称
程序集是托管代码程序的部署和标识单元。 尽管程序集可跨一个或多个文件，但通常程序集与 DLL 相互映射。 因此，本节仅介绍 DLL 命名约定，然后可以将其映射到程序集命名约定。

 ✔️为程序集 Dll 选择名称，这些名称建议了大块功能，如 System.object。

 程序集和 DLL 的名称不必与命名空间名称对应，但在命名程序集时遵循命名空间名称是合理的。 合理的经验法则是基于程序集中包含的命名空间的公共前缀来命名 DLL。 例如，可以调用具有两个命名空间和的程序集 `MyCompany.MyTechnology.FirstFeature` `MyCompany.MyTechnology.SecondFeature` `MyCompany.MyTechnology.dll` 。

 ✔️考虑根据以下模式命名 Dll：

 `<Company>.<Component>.dll`

 其中 `<Component>` 包含一个或多个以句点分隔的子句。 例如：

 `Litware.Controls.dll`.

 *部分©2005，2009 Microsoft Corporation。保留所有权利。*

 *皮尔逊教育，Inc. 的经许可重印权限[：从框架设计指导原则：用于可重复使用的 .Net 库的约定、惯例和模式、第2版](https://www.informit.com/store/framework-design-guidelines-conventions-idioms-and-9780321545619)By Krzysztof Cwalina 和 Brad Abrams，发布十月22，2008，作为 Microsoft Windows 开发系列的一部分。*

## <a name="see-also"></a>另请参阅

- [框架设计准则](index.md)
- [命名准则](naming-guidelines.md)
