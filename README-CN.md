[**简体中文**](./README-CN.md) | [English](.//README.md)

# 欢迎来到适用于 Linux 的 Windows 子系统（WSL）仓库

<p align="center">
  <img src="./Images/Square44x44Logo.targetsize-256.png" alt="WSL logo"/>
</p>

[了解更多关于 WSL](https://aka.ms/wsldocs) | [下载与发布说明](https://github.com/microsoft/WSL/releases) | [为 WSL 做贡献](./CONTRIBUTING.md)

## 关于

适用于 Linux 的 Windows 子系统（WSL）是一种强大的方式，可让你在 Windows 上直接运行 Linux 的命令行工具、实用程序和应用程序——全部无需修改、直接运行，而且没有传统虚拟机或双系统启动所带来的额外开销。
你可以直接在 Windows 命令行中运行以下命令来立即安装 WSL：

```powershell
wsl --install
```

你可以通过[安装最佳实践](https://learn.microsoft.com/windows/wsl/setup/environment)、[WSL 概览](https://learn.microsoft.com/windows/wsl/about)以及我们的 [WSL 文档页面](https://learn.microsoft.com/windows/wsl/)了解更多信息。

## 相关仓库

WSL 还拥有相关的开源仓库：

- [microsoft/WSL2-Linux-Kernel](https://github.com/microsoft/WSL2-Linux-Kernel) - 随 WSL 一同发布的 Linux 内核
- [microsoft/WSLg](https://github.com/microsoft/wslg) - 为 WSL 提供 Linux GUI 应用支持
- [microsoftdocs/wsl](https://github.com/microsoftdocs/wsl) - 位于 aka.ms/wsldocs 的 WSL 文档

## 贡献

本项目欢迎各种形式的贡献，包括编码功能、缺陷修复、文档修正、设计提案等。

在开始贡献之前，请先阅读我们的[贡献者指南](./CONTRIBUTING.md)。

如需 WSL 开发方面的指导，请阅读[开发者文档](./doc/docs/dev-loop.md)，其中包含如何从源代码构建 WSL 的说明以及其体系结构的详细信息。

## 行为准则

本项目已采用[微软开源行为准则](./CODE_OF_CONDUCT.md)。

## 商标

本项目可能包含项目、产品或服务的商标或徽标。对微软商标或徽标的授权使用须遵循[微软商标与品牌准则](https://www.microsoft.com/legal/intellectualproperty/trademarks)。在本项目的修改版本中使用微软商标或徽标不得造成混淆，也不得暗示微软的赞助。任何第三方商标或徽标的使用均须遵循相应第三方的政策。

## 隐私与遥测

本应用程序会记录基本的诊断数据（遥测）。有关隐私及我们收集哪些数据的更多信息，请参阅我们的[数据与隐私文档](DATA_AND_PRIVACY.md)。

本软件可能会收集有关你以及你对本软件的使用情况的信息，并发送给微软。微软可能会使用这些信息来提供服务并改进我们的产品和服务。你可以按照仓库中的说明关闭遥测。本软件中的某些功能还可能使你与微软能够从你应用程序的用户处收集数据。如果你使用这些功能，则必须遵守适用的法律，包括向你的应用程序用户提供适当的通知，并附上微软隐私声明的副本。我们的隐私声明位于 https://go.microsoft.com/fwlink/?LinkID=824704。你可以在帮助文档和我们的隐私声明中进一步了解数据的收集与使用。你使用本软件即表示你同意这些做法。

## 关于本地化的说明

WSL 中所有关键的 CLI 文本均已本地化，但部分详细的错误输出尚未完全本地化。具体来说，在 `wslc.exe` 中我们使用了一些不具备完整本地化支持的底层开源库。我们在错误输出中保留了这些未本地化的字符串，以便提供更丰富的故障上下文，使最终用户能够更容易地解决问题。
