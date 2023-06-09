# 如何将 Google AdSense 添加到 WordPress

> 原文：<https://medium.com/visualmodo/how-to-add-google-adsense-to-wordpress-f844556230bb?source=collection_archive---------6----------------------->

了解如何以一种简单的方式在你的 WordPress 网站上添加 google AdSense，并完全设置它以获得更好的使用、控制和结果。

在本教程中，您将学习:

*   如何在您的 AdSense 帐户中验证您的网站？
*   如何激活站点授权，防止不属于你的站点滥用你的 AdSense 代码？
*   如何为移动和桌面访问者添加自动放置的 AdSense 广告(称为页面级广告)。
*   如何测试 AdSense 页面级广告？

按照 Google AdSense 政策，请确保您有一个经过批准的 AdSense 帐户，并且在您的网站上有适当的隐私和 Cookie 政策信息。

![](img/3f9e3c4d51e3aaea9e2aed2de7fc674f.png)

首先，让我们验证你的网站。如果想要使用快速入门功能，这是一个必需的步骤。QuickStart 允许自动、智能地为您网站的移动和桌面访问者放置 AdSense 广告。

1.  要验证您的网站，请在您的 Google AdSense 帐户中，单击“设置”,然后单击“我的网站”。
2.  单击加号按钮。
3.  在框中键入您的网站地址。
4.  单击添加站点。

在这一点上，你可能想设置它，以便*只有*你的授权网站可以显示你的 AdSense。

有时候，另一个网站会抓取你的网站内容，包括你的 AdSense 代码，然后将这些内容添加到他们的网站上。

如果发生这种情况，并且该网站违反了任何谷歌广告政策，那么受影响的就是你。这一步只是防止你希望你已经做得更快，如果这样的事情发生了。

# 要设置站点 AdSense 授权:

1.  在“管理站点”区域，单击页面右侧的 3 个堆叠点。
2.  点击站点授权。
3.  将其打开，然后单击“保存”。

现在，让我们在您的网站上激活广告的自动放置。

# 要打开此功能:

1.  在您的 AdSense 帐户中，进入我的广告，然后页面级广告。
2.  通过滑动滑块，打开锚定/覆盖广告和插页广告中的一个或两个。
3.  在新的标签页或窗口中打开你的 WordPress 仪表盘。

![](img/69c694ce64f0e281ea061ff1fdb9cf58.png)

下一步是获取您的网站所需的代码，以完成设置。

值得注意的是，这段代码与新的 google ads 用户在申请过程中需要添加到他们网站的代码是一样的。因此，您可能已经准备好了，可以跳到测试部分。

谷歌广告的长期用户不需要在申请时放置这些代码，所以这些步骤将是必需的。

此外，值得一提的是，这完全相同的代码可以用在所有网站的所有页面上。

下一步，我们将创建一个快速插件，将 AdSense 代码放在 WordPress 网站的所有页面上。

我发现使用 Pluginception 插件安装一个插件非常简单快捷，所以让我们先把它安装好。

# 要安装 Pluginception，请按照下列步骤操作:

1.  在你的 WordPress 仪表盘中，点击插件，然后点击添加新的。
2.  在搜索框中，键入 [Pluginception](https://wordpress.org/plugins/pluginception/) 。
3.  单击立即安装。
4.  单击激活。这将在插件菜单中打开一个名为创建新插件的新选项。

# 按照以下步骤创建您的自定义插件:

1.  单击创建新插件链接。
2.  给插件起一个名字，比如我的谷歌广告放置插件。
3.  单击创建空白插件按钮。
4.  现在，将你在视频中看到的代码添加到你的插件中，或者在这些步骤下面，如果你是按照书面教程进行的话。
5.  切换回 AdSense。
6.  单击获取代码按钮。
7.  将代码复制到剪贴板。
8.  用上一步从 AdSense 复制的代码替换显示您的 ADSENSE 代码的地方。
9.  单击更新文件按钮。

有两种方法可以测试你的工作。让我们现在两样都做。

1.  从您的台式机或笔记本电脑访问您的网站。
2.  右键单击页面上的任意位置，然后单击查看源代码。
3.  查找您插入的代码。你可以做一个查找，通常是通过按 Ctrl+F 并键入 adsbygoogle 作为一个没有空格的单词。
4.  现在，让我们来看看广告是否在手机上显示。使用高端移动设备在纵向视图(与横向视图相反)下打开网站页面。将#googleads 添加到 URL 的末尾。
5.  选择您要测试的广告格式，然后在您的设备上检查结果。
6.  对于插页，单击页面上任何突出显示的链接来测试广告是否有效。

如果你在测试中遇到显示广告的问题，一定要访问谷歌的页面级广告测试指南，看看为什么会这样。在谷歌上搜索“页面级广告测试指南”来找到这个页面。

# 本教程中使用的代码:

```
function my_google_adsense_placement_function() {
  $output='YOUR ADSENSE CODE';
  echo $output;
}
add_action('wp_head','my_google_adsense_placement_function');
```

所有的 [Visualmodo WordPress 主题](https://visualmodo.com/)都有一个定制区域，在主题选项上可以方便地上传代码，如果你想用另一种方式，两种方式都可以很好地工作。