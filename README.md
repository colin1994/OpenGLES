# OpenGL ES， 初学者的自我总结

> 前言：
>
> 学习 OpenGL ES 一段时间了，**深知这个过程的不容易**。
>
> 尤其是入门，OpenGL 到底好在哪里？什么是渲染管线？什么是状态机？纹理是不是就是图片？深度测试，模版测试又是什么鬼？...
>
> OpenGL **有太多太多的东西需要学习**。我最初接触 OpenGL，就是想借助它，实现美图秀秀里的一些功能。然而，不知道看了多少教程，实现了多少个旋转立方体，困惑了多少次，放弃了多少回...
>
> 慢慢地，似乎找到了一些门路...
>
> * 可以导入照片处理并保存了
> * 可以实现简单的滤镜了
> * 可以实现画笔功能了
> * 可以实现马赛克功能了
> * ...
>
> 于是，这系列的文章应运而生。





## 目标

这系列文章主要是个人学习过程中的一些总结，因为本人也是初学者，所以会从初学者角度，介绍 OpenGL ES 图像处理最直接的一些知识。

**利用 OpenGL ES，学习如何在 iOS 平台上进行图像处理，实现各种效果。**

这，就是我想学到的，也是想分享给大家的。



> PS：时间允许的话，希望能保证一个星期输出一篇文章，鞭策自己～



## 目录

### 基础扫盲：

1. [OpenGL ES 开篇](/Lesson00) : 以 Q&A 的形式，列举出在学习 OpenGL ES 之前会存在的一些疑惑。权衡是否该继续学习 OpenGL ES。
2. OpenGL ES 基础概念：扫盲篇，先介绍一些必须了解的知识，便于之后能直接进入实战阶段。
3. OpenGL ES 环境搭建：详解 OpenGL ES 接入方式，以最基础效果（设置背景色）来阐述。
4. 渲染基本图元，三角形：详细介绍可编程图形渲染管线是如何工作的。
5. GLSL 全解：详细介绍 OpenGL ES 2.0 着色器语言 GLSL。




### Demo 讲解：

1. 显示图片
2. 视图封装
3. 滤镜：色温（简单全局应用）
4. 滤镜：Vignette，晕映（根据距离，区分处理）
5. 形变：马赛克（简单形变，几点汇聚成一点）
6. 形变：素描效果（根据边缘点，动态计算取样点色值）
7. 基于 Lookup Table（Lut）的滤镜实现（用查找表替代浮点计算，提高效率）
8. 多重滤镜叠加（实现及优化）




### 实战训练：

>敬请期待






## 学习资料

> PS：这里将罗列个人学习过程中，认为好的一些书籍，教程，Demo等。
>
> 该系列的文章中，一些阐述，配图，可能是从其它文章或者书籍中摘录整理的。为保证阅读以及书写方便，这部分出处说明统一放到学习资料里。
>
> 本人也处于学习阶段，精力有限，难免引用前人优秀教程。如果对您造成不必要的麻烦，请及时告知。



### 书籍

[OpenGL ES 2.0 API 快速参考卡片](https://www.khronos.org/opengles/sdk/docs/reference_cards/OpenGL-ES-2_0-Reference-card.pdf)

[红宝书：OpenGL Programming Guide](https://www.amazon.com/OpenGL-Programming-Guide-Official-Learning/dp/0134495497)

[蓝宝书：OpenGL Superbible](https://www.amazon.com/OpenGL-Superbible-Comprehensive-Tutorial-Reference/dp/0672337479)



### 教程

[OpenGL ES Programming Guide for iOS](https://developer.apple.com/library/content/documentation/3DDrawing/Conceptual/OpenGLES_ProgrammingGuide/Introduction/Introduction.html#//apple_ref/doc/uid/TP40008793-CH1-SW1)

[Learn OpenGL](http://learnopengl.com/)

[OpenGL ES_Max](http://www.edwinho.org/lessons/2015-08/opengl-es.html)

[OpenGL ES 01 OpenGL ES之初体验](http://blog.csdn.net/kesalin/article/details/8221393)



### Demo

[GLImageProcessing](https://github.com/twenty3/GLImageProcessing)

[GPUImage](https://github.com/BradLarson/GPUImage)

[BCMeshTransformView](https://github.com/Ciechan/BCMeshTransformView)



### Idea

[Shadertoy](https://www.shadertoy.com/)

[PhotoFunia](https://photofunia.com/)





> PS：本人也处于 OpenGL ES 学习阶段，所以文章中**难免存在问题**，或者待优化地方。如果有任何不对，**欢迎指出交流**～