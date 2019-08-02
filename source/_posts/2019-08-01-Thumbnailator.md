---
title: Thumbnailator
categories:
  - Java
  - Thumbnailator
tags:
  - images
mp3: ''
cover: 'http://likoli.cn/imgs/file_1564729383000_cbcc21ec5dacb4c1bf9131cacd7f2e3f.jpg'
date: 2019-08-01 19:50:19 
---

# Thumbnailator

## 什么是Thumbnailator？

{% asset_img home-image.png home image %}

*Thumbnailator* 是Java写的一个缩略图生成包

## 为什么要用Thumbnailator？

在Java中制作高质量的缩略图可能是一项相当困难的任务。

需要学习如何使用 Image I/O API, Java 2D API, 图片处理，图片缩放技术…, 不要担心！ *Thumbnailator* 将为我们处理所有这些事情!

*Thumbnailator* 是一个单独的JAR文件并且不依赖任何外部包，使开发和部署变得简单容易。为了简单的被引入到Maven项目中, 你可以在Maven Central Repository 中获取到它。

## Thumbnailator有多简单？

*Thumbnailator*'s流式接口可以用来在一个简单的步骤中处理进行相当复杂的图片缩略任务。

举个例子, 为一个目录中的图片文件创建JPEG缩略图，全部调整为640像素×480像素的最大尺寸，同时保留原始图像的纵横比可以通过以下方式执行：

```Java
Thumbnails.of(new File("path/to/directory").listFiles())
    .size(640, 480)
    .outputFormat("jpg")
    .toFiles(Rename.PREFIX_DOT_THUMBNAIL);
```

*Thumbnailator*提供的流式接口将制作缩略图的任务变成了一个简单的方法调用！

不需要访问Image I/O API 和 通过`Graphics2D`来手工操作`BufferedImage`

*Thumbnailator*能为你做所有的这些事情。

## Thumbnailator能做什么？

想知道Thumbnailator能做什么, 你可以访问下面这些页面:

- [Features](https://github.com/coobird/thumbnailator/wiki/Features)
- [Examples](https://github.com/coobird/thumbnailator/wiki/Examples)
- [Thumbnailator API Documentation](https://coobird.github.io/thumbnailator/javadoc/0.4.8/)

## 免责声明

*Thumbnailator仍处于早期开发阶段，API随时可能发生变化。*