---
layout: post
title:  "eclipse导入maven工程 missing artifact / can not be resolved（实际是存在的)"
categories: exceptions
tags: eclipse maven artifact
author: DooWhop
---

* content
{:toc}

 最近切换maven仓库还有eclipse, 通过svn或者git引入工程, 莫名报missing artifact / can not be resolved等错误, 查看Maven Dependencies这些报错的包都存在,最后解决方法如下:




> 找到出错的jar包文件位置或者在仓库文件夹下检索所有包，删掉_maven.repositories和_remote.repositories文件，然后update project。

[参考]

-[关于maven仓库中的_remote.repositories](https://my.oschina.net/yibuliushen/blog/1550292)

-[eclipse导入maven工程missing artifact（实际是存在的）错误解决](https://www.cnblogs.com/zxy500/p/5836044.html)

如果以上方法仍没解决,请参考:

-[Maven2: Missing artifact but jars are in place](https://stackoverflow.com/questions/6111408/maven2-missing-artifact-but-jars-are-in-place)

-[解决Maven的“Missing artifact ……”](https://www.jianshu.com/p/510874e47dea)
