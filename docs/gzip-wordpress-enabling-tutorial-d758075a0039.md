# GZIP WordPress 授权教程

> 原文：<https://medium.com/visualmodo/gzip-wordpress-enabling-tutorial-d758075a0039?source=collection_archive---------0----------------------->

速度是每个网站所有者的愿望清单上的第一位。站点越快，体验越好，转化越多。此外，谷歌在搜索结果中将加载速度更快的页面排在更高的位置。所以你有一个很好的理由从你的网站上尽可能地挤出最后一毫秒。GZIP 提出了一种优化 WordPress 网站速度的特殊方法。让东西加载更快的最好方法就是让它们更小。

![](img/b8ae5896970853d9b94137eea5c087a5.png)

这正是 GZIP 所做的。我们将向您展示如何启用它，并确保您的页面速度极快，即使您已经设置并优化了[图像压缩](https://visualmodo.com/images-compression-site-loading/)和其他设置。

# GZIP 新闻压缩

GZIP 是一个优化的文件格式和文件压缩和解压缩软件 aa。让-卢普盖利和马克阿德勒创造了 GZIP 压缩。它的免费软件减少了旧系统。

和 WordPress 核心软件一样，GZIP 被用于 GNU(自由开源软件)。“G”来自“GNU”WordPress GZIP 压缩是减少网站文件大小的过程，包括 HTML、CSS 和 JavaScript 等代码。

GZIP 技术对图像不起作用。然而，当涉及到媒体文件时，它就是一个袋子。例如，一些图像文件，如 MPEG 和 WAV 文件，使用 GZIP 可以很好地压缩，而其他文件类型，如音频文件夹，如果您尝试压缩它们，其大小可能会增加。

必须在您的 web 服务器上启用 GZIP 压缩，您才能启用文件和文件夹压缩(启用了 GZIP 的 web 服务器将在其响应中返回内容编码:GZIP 标头)。

从客户端来看，所有现代的 web 浏览器都支持 GZIP 压缩，并在发出 HTTP 请求时自动要求进行压缩——这意味着一旦启用了 GZIP 压缩，所有用户都可以从中获益。

# 启用 GZIP 压缩

有两种方法可以启用 GZIP 压缩:修改。htaccess 文件或者使用 WordPress 插件，比如 WP Rocket。使用 WordPress 插件，在你的 WordPress 站点上启用 GZIP 压缩最简单的方法就是安装一个插件。这将比修改。htaccess 文件。有很多插件可供选择，但我们选择了这三个 WP 插件，因为它们的特点和易用性:

# WP-优化

提升网站性能的一体化解决方案。该插件将启用 GZIP 压缩和网页缓存。除此之外，它还会清除网站上不必要的文件。这个工具甚至可以优化图像来释放更多的空间！

# 蜂鸟

你有更多的自由来选择你想要优化的方面。GZIP 压缩，缩小和屏幕外图像的惰性加载是它的一些主要功能。

# WP 最快的缓存

WP 最快缓存结合其缓存实力与 GZIP 压缩，使您的页面快速和轻量级。这个工具还可以自动禁用表情符号，优化每一个帖子。

由于这些插件能做的不仅仅是启用 GZIP 压缩，我建议你尝试所有的插件，看看哪一个最适合你。毕竟都是免费的，频繁更新，有什么不喜欢的？

这种方法技术性很强，所以更适合高级用户。但是，只要细心，谁都可以做到。在我们继续之前，请记住您应该始终备份您的。htaccess 文件，如果出现错误。

# 。htaccess

您需要下载一个 FTP 客户端，比如 Filezilla，来定位。htaccess 文件。它通常出现在你的网站的 public_html 索引中。下载该文件，并在您的计算机上保存一份副本作为备份。然后，在. htaccess 的# END WordPress 行之前粘贴以下代码。

将编辑过的文件上传到同一位置。如果 FileZilla 请求覆盖它，请单击“确定”。