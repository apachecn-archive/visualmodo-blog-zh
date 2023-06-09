# 如何自动化你的 API 测试过程

> 原文：<https://medium.com/visualmodo/how-to-automate-your-api-testing-process-1f767e7ab795?source=collection_archive---------0----------------------->

在本文中，我们将分享和探索自动化 API 测试过程的最佳方法。在软件应用的创建中使用应用编程接口或 API 是全球软件开发社区中的普遍做法。这主要是因为 API 允许开发者有效且容易地定义他们的应用程序的独立软件组件如何以标准化语言相互通信。因此，开发人员可以自由地专注于提炼使他们的应用程序独特和创新的东西，而不是从头开始编写接口代码。

# API 测试的重要性

![](img/9d02731ba77c31e54da76bf8bbc6d9e2.png)

这种在软件开发中的广泛使用和集成使得 API 测试变得更加重要。除了确保应用程序的基本组件正常运行之外，API [测试](https://visualmodo.com/ultimate-guide-ab-testing-infographic/)还有助于根除 API 中的关键错误和缺陷，这些错误和缺陷通常会对应用程序的性能和功能产生负面影响。这些错误可能包括安全漏洞、无法处理错误类型的数据输入或大量负载等等。

# API 测试的挑战以及 API 自动化如何解决它们

然而，手动测试所有这些可能是一个相当大的挑战，因为您需要编写一个单独的应用程序来测试每一个潜在的问题。如果你的开发进度很紧，没有太多的余地，这一点尤其正确。

在这种情况下，自动化 API 测试是更有效的选择。自动化 API 测试涉及到工具的使用，这些工具可以被编程来自动执行重复性测试。当您选择运行一个全面的 API 测试工具来执行您的 API 测试时，您可以在监视结果的同时自由地做其他开发任务。这使得开发周期更加敏捷和高效。

# 自动化 API 测试的八个简单步骤

为了在这方面帮助您，这里有一个简单的分步指南，介绍如何自动化您的 API 测试过程，使用一个 API 执行和自动化测试用例进行基本的 API 功能测试。

# 1 选择一个全面的测试工具

网上有很多 API 自动化测试工具。它们中的大多数都提供了类似的特性，并增加了一些额外的功能来帮助您的测试更加方便。有些，像 Postman，可以免费使用，而有些则被锁在收费墙后面。无论你选择哪一个，在使用之前都要检查它是否符合你的测试要求。

# 2 选择方法类型并输入 API URL

因为这是一个功能测试——即确保 API 本身工作——我们需要选择相关的方法并输入 API 的 URL。寻找你选择的工具的 API runner 特性，选择你想要的方法，输入被测试的 API 的 URL。

# 3 为 API 请求添加附加信息

为了成功地运行请求，可能会出现一些额外的参数，比如头、主体等等。要添加这些参数，请在 API runner 窗口中查找 parameters 选项卡，然后单击 Add Parameter test 按钮，或者您选择的 API 自动化工具中的等效按钮。然后，您将看到一个字段，用于添加所需的键和参数值。

# 4 输入认证凭证

当您的托管 API 要求在运行请求之前进行身份验证时。您应该首先输入所需的凭据。您选择的 API 自动化工具应该有一个 Authorization 选项卡，允许您从下拉列表中选择身份验证类型。这将为您提供输入用户名和密码的字段。

# 5 个输入断言

接下来，您需要向测试中添加断言。断言允许您指定 API 在测试过程中应该响应哪种数据或信息。如果 API 没有提供断言所要求的那种响应。测试本身可能会失败。转到工具的 API Runner 窗口中的 Assertion 选项卡。此外，从下拉列表中选择响应和断言条件。然后在值字段中输入值。要添加更多的断言，只需点击 Add Assertions 按钮或自动化工具中的等效按钮。

# 6 个输入变量

最后，向测试中添加变量允许您存储 [API](https://en.wikipedia.org/wiki/Web_API) 在响应测试请求时发送的值。然后，您可以将这些值用作后续测试的预期断言。因此，允许更完整的功能测试体验。要添加变量，只需转到自动化工具中的 Variables 选项卡。此外，输入变量名和值的 JSON 路径，作为 API 响应的数据。要添加更多变量，您也可以单击添加变量按钮或等效按钮。

# 7 运行 API 请求并检查结果

开始测试前，对所有东西进行最后一次检查。这将把测试保存到工具的内存中并运行它。您应该能够运行相同的测试，而不必输入所有以前的值，并且可以在 API 执行历史中看到结果。

# 8 必要时重复 API 测试过程

使用 API 测试工具进行新的测试，并根据需要重复测试，以获得您需要的结果。随着最后一步的完成。您已经使用 API 测试工具成功地自动化了单个 API 测试用例。现在，您已经准备好以更高的强度和重复次数运行测试，以真正改进和完善您的应用程序。