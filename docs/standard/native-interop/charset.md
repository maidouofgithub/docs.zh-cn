---
title: 字符集和封送 - .NET
description: 了解字符集的不同值如何更改 .NET 将数据封送到本机代码的方式。
ms.date: 01/18/2019
ms.openlocfilehash: 4be4bd5a968eb5c0d6959a0f378ee1223ed906ed
ms.sourcegitcommit: 5f236cd78cf09593c8945a7d753e0850e96a0b80
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "75706382"
---
# <a name="charsets-and-marshaling"></a>字符集和封送

`char` 值、`string` 对象和 `System.Text.StringBuilder` 对象的封送方式取决于 P/Invoke 或结构上的 `CharSet` 字段的值。 可以通过在声明 P/Invoke 时设置 <xref:System.Runtime.InteropServices.DllImportAttribute.CharSet?displayProperty=nameWithType> 字段来设置 P/Invoke 的 `CharSet`。 若要设置 `CharSet` 类型，请在类或结构声明中设置 <xref:System.Runtime.InteropServices.StructLayoutAttribute.CharSet?displayProperty=nameWithType> 字段。 未设置这些属性字段时，将由语言编译器确定使用哪些 `CharSet`。 C# 和 Visual Basic 默认使用 <xref:System.Runtime.InteropServices.CharSet.Ansi> 字符集。

下表显示了每个字符集之间的映射以及字符或字符串在使用该字符集封送时的表示形式：

| `CharSet` 值 | Windows            | Unix 上的 .NET Core 2.2 及更低版本 | Unix 上的 .NET Core 3.0 及更高版本和 Mono |
|-----------------|--------------------|-----------------------------------|------------------------------------------|
| Ansi            | `char`（系统默认的 [Windows (ANSI) 代码页](/windows/win32/intl/code-pages)）      | `char` (UTF-8)                    | `char` (UTF-8)                           |
| Unicode         | `wchar_t` (UTF-16) | `char16_t` (UTF-16)               | `char16_t` (UTF-16)                      |
| 自动            | `wchar_t` (UTF-16) | `char16_t` (UTF-16)               | `char` (UTF-8)                           |

确保了解选择字符集时所需的本机表示形式。
