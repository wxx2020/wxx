---
title: "第1章 R语言入门"
date: 2021-12-13T21:47:01+08:00
draft: true
description:
categories:
 - R
featured_image:
author: "wxx"
---


> **学习目标：**
>
> 1. 学会R和RStudio的获取和安装，能够对RStudio进行自定义设置；
> 2. 了解R语言的发展历史、特点以及与其他软件相比的优劣势；
> 4. 熟练掌握R包的安装和加载，能够快速查看相应的帮助文档；
> 4. 学会常用的快捷键操作，形成自己的代码编写风格。

为了方便读者的学习，本书在讲解过程中会穿插补充一些内容，包括对文中内容的解释或扩展、提示读者注意、补充的作业任务和使用小技巧等。这些内容将会采用注释的形式出现，本书采用不同的[emoji](https://www.webfx.com/tools/emoji-cheat-sheet/)符号开头从而对注释内容加以分辨：

- :pushpin:表示对相关内容的进一步解释或扩展，通常针对的是出现在上一段的内容；
- :loudspeaker: 表示注释内容需要读者注意，通常是新手在初次使用时经常出现的错误；
- :pencil:表示需要读者亲自尝试完成的补充作业，以加深读者对相关内容的理解；
- :key:表示在使用R语言时的一些小技巧，掌握这些小技巧通常能够提高工作效率。

## 1.1 初识R语言

### 1.1.1 R语言的性质、功能和特征

R语言是什么？这或许是许多新手在第一次接触R语言最想搞清楚的问题。根据[R语言官网](https://www.r-project.org/)的介绍：`R is a free software environment for statistical computing and graphics`，也就是说，R是用于统计计算和制图的自由软件环境。这个介绍虽然简短，但同时点明了R语言的性质、功能和特征。

R语言的性质是一种[解释型编程语言](https://baike.baidu.com/item/%E8%A7%A3%E9%87%8A%E5%9E%8B%E8%AF%AD%E8%A8%80/8888952?fr=aladdin)环境，在使用时主要依靠编写代码或脚本来执行命令从而获取相应的结果。“环境”则意味着R语言是一个完善且统一的系统，它不仅可以提供一些集成的统计工具，更大量地提供各种统计计算的函数，从而使得用户能够灵活地进行数据分析，甚至创造出符合需要得新的统计计算方法（王斌会，[2017](https://book.douban.com/subject/27106145/)）。

R语言的主要功能在于统计计算和制图，作为统计分析工具，R语言几乎覆盖了整个统计领域的前沿算法，经典的回归分析和火爆的神经网络都可以通过直接调用函数来实现，在制图方面，R语言能够以一种简单而直接的方式创建优雅、 信息丰富、高度定制化的图形（见[图1](#1-plots)）(朱雪宁 等，[2018](https://book.douban.com/subject/30395816/)；Robert Kabacoff，[2016](https://book.douban.com/subject/26785199/))。除上述主要功能之外，丰富的R包使得R语言在数据管理、大数据分析、程序开发等方面也有不俗的表现。

R语言最显著的特征是自由，这得益于它的免费、开源和易扩展性，相比于传统的商业统计软件，R语言可以免费下载任何有关的安装程序、源代码、程序包及其源代码、文档资料，其源代码托管在[Github](https://github.com/SurajGupta/r-source)，任何用户都可以直接接触到。R语言包含大量的扩展包并且拥有方便的二次开发功能，与其他各种语言（例如[Python](https://baike.baidu.com/item/Python/407313?fr=aladdin)，[C](https://baike.baidu.com/item/c%E8%AF%AD%E8%A8%80/105958?fr=aladdin)）都可以无缝对接。这些特点使得R语言受到了统计专业人士的青睐，成为当前应用最为广泛的数据统计分析软件之一。

<center>
    <figure>
    <img src="https://gitee.com/dolphinxi/picbed/raw/master/unnamed-chunk-1-1.png" width="373"/>
    <img src="https://gitee.com/dolphinxi/picbed/raw/master/299-circular-stacked-barplotBig.png", width="373"/>
    <img src="https://gitee.com/dolphinxi/picbed/raw/master/Surfer_travel.png", width="750"/>
    </figure>
    <span id="1-plots">图1：R语言制图示例（来源：https://www.r-graph-gallery.com/index.html）</span>
</center>

### 1.1.2 R语言的发展历史

R语言起源于另一门语言——[S语言](https://www.whoishostingthis.com/resources/s-plus/)，是S语言的一个变种。S语言是由AT&T[贝尔实验室](https://baike.baidu.com/item/贝尔实验室)的John Chambers等人于1976年开发的一种用来进行数据探索、统计分析、作图的[解释型语言](https://baike.baidu.com/item/解释型语言)。[^1]它目前有两种实现版本：一种是由TIBCO经营的商业软件S-plus；另一种就是免费开源的R语言。

1992年，Auckland大学的[Ross Ihaka](https://www.stat.auckland.ac.nz/~ihaka/)和[Robert Gentleman](https://www.computerhope.com/people/robert_gentleman.htm)（见[图2](#1-creator)）为了能够更有效地开展大学统计入门课程的教学，决定引入S语言来开发一套软件。由于他们两个人的名字都是以字母R开头的，所以他们将这款软件称为R语言。1994年R语言的雏形基本形成，在同行的鼓励下，他们决定采用自由软件基金会的通用公共许可证（GPL）将R语言作为一款自由软件发布。1997年，Kurt Hornik和Fritz Leisch在维也纳建立了[R综合档案网络](https://cran.r-project.org/)（Comprehensive R Archive Network，简称CRAN）作为用户贡献的存储库。2000年2月29日，基本功能齐全且足够稳定的R语言1.0版本正式发布。[^2]此后，越来越多的用户提供了各式各样的R扩展包，使得R语言的功能日益丰富且强大。截至2021年4月12日，CRAN上发布的扩展包已经达到17422个，且近年来呈现出递增的趋势（见[图3](#1-pkgnumber)）。

<center>
    <figure>
    <img src="https://gitee.com/dolphinxi/picbed/raw/master/ross-ihaka.jpg" width="150"/>
    <img src="https://gitee.com/dolphinxi/picbed/raw/master/robert-gentleman.jpg", width="150"/>
    </figure>
    <span id="1-creator">图2：R语言创始人Ross Ihaka（左）和Robert Gentleman（右）</span>
</center>
<center>
    <figure>
    <img src="https://gitee.com/dolphinxi/picbed/raw/master/plot.png", width="750"/>
    </figure>
    <span id="1-pkgnumber">图3：2006-2020历年CRAN上发布的R包数量</span>
</center>


> :pushpin:除R 语言之外，C语言也是贝尔实验室的一项重要研究成果，但两者有不同的侧重领域，R 语言是一种解释型的面向数学理论研究工作者的语言，而 C 语言是为计算机软件工程师设计的。如果你是一个计算机程序的初学者并且急切地想了解计算机的通用编程，R 语言不是一个很理想的选择，可以选择 Python、C 或 Java。
>
> R 语言是解释运行的语言（与 C 语言的编译运行不同），它的执行速度比 C 语言慢得多，不利于优化。但它在语法层面提供了更加丰富的数据结构操作并且能够十分方便地输出文字和图形信息，所以它广泛应用于数学尤其是统计学领域。[^3]

[^1]:关于S语言的更多内容请查看：https://baike.baidu.com/item/S%E8%AF%AD%E8%A8%80/2440117?fr=aladdin。

[^2]:关于R语言发展历史的更多内容请查看：https://www.stat.auckland.ac.nz/~ihaka/downloads/Massey.pdf和https://cran.r-project.org/doc/html/interface98-paper/paper_2.html。
[^3]:参考资料来源：https://www.runoob.com/r/r-tutorial.html。

### 1.1.3 R语言的优势与缺点

R语言是由数据处理、统计计算和图形绘制等一系列工具组成的集成软件，它的功能特点主要体现在：

1. 有效的数据处理和保存机制；
2. 拥有一整套数组和矩阵的操作运算符；
3. 拥有一系列大型、连贯且完整的数据分析中间工具；
4. 可以直接对数据进行分析和展示的图形设备；
5. 是一种发展完善、简洁高效的程序设计语言，包括了条件语句、循环语句、用户自定义的递归函数以及输入输出接口。[^4]

除了R语言之外，我们还经常见到[Stata](https://www.stata.com/)、[SAS](https://www.sas.com/)、[SPSS](https://www.ibm.com/analytics/spss-statistics-software)、[Matlab](https://www.mathworks.com/products/matlab.html)等同类软件，为什么不选择这些软件而选择R语言呢？这是因为R语言有着非常多的值得尝试的优势：

1. 免费、开源、跨平台。与常见的商业软件相比，R语言不需要昂贵的价钱购买或维护，可以直接免费下载和使用，对于教师和学生来说，这种好处是显而易见的。R语言的开源性使得它具有强大的发展潜力，自从它被开发出来至今，讨论开发R的综合网站和R的附加模板一直层出不穷，大大方便了各类研究人员。此外，R语言可以在各种操作系统上使用，无论是常用的Windows、MacOS还是少见的Linux，甚至可以通过在服务器上搭建 RStudio Server来实现不同终端的跨平台登陆使用。
2. 小巧轻便、运行速度快。与动辄几个GB的Matlab和SAS等统计软件相比，R语言更加小巧轻便，最新的R4.0.5的安装包近有84.4MB，可以在1-2秒内启动并投入使用（当然，这与你的电脑配置也有关系）。R语言更新速度相对较快，可以抢先囊括其他软件中尚不可用的、先进的统计计算例程，有些新方法的更新速度是以周来计算的。尽管小巧，但R语言的运行速度却丝毫不逊色于其他软件，github上有个项目（[benchmark-stata-r](https://github.com/matthieugomez/benchmark-stata-r)）专门比较了在同一台电脑的Stata和R中进行相同数据操作程序所花费的时间，结果表明R语言整体上要优于Stata。
3. 强大的数据处理、统计分析和图形绘制功能。截至目前，R用户社区已提供了超过1.7万的功能扩展包，涵盖了小样本概率估计、时间序列、贝叶斯分析、复杂抽样数据统计、神经网络、空间地理分析、网络爬虫、非结构化数据分析等诸多统计领域。依托辅助的扩展包，R语言可以轻松地从各类数据源获取数据并将其转化为可用的形式，并完成数据的整理、转换、建模、可视化以及结果沟通，分析步骤的结果均可被轻松保存到不同的文件系统中。R语言拥有顶尖水准的制图功能（如[图1](#1-plots)所示），除了自身所带的画图工具外，还有强大的**lattice**包和**ggplot2**包。总而言之，扩展包既是R语言开放性和易拓展性的具体体现，也是R语言卓越功能的动力源泉。
4. 活跃的社区和丰富的资源。作为一款开源软件，R语言背后有一个强大的用户社区和大量的开放资源，获取帮助非常容易。国外比较活跃的R用户社区有[GitHub](https://github.com/)和[Stack Overflow](https://stackoverflow.com/)等，R包的开发者通常会将代码放到Github，接受使用者的问题和建议，等代码成熟后再发布到CRAN上；而Stack Overflow则是一个优质的开发者问答网站，R语言使用过程中出现的许多问题都可以尝试在此找到答案。国内最活跃的R用户社区当属[统计之都](https://cosx.org/)以及统计之都旗下的[COS论坛](https://d.cosx.org/)，这些网站对R语言用户都具有很高的参考价值。此外，[B站](https://www.bilibili.com/)有许多针对初学者的免费的学习视频，而关于R语言学习的英文书籍可以尝试在[bookdown](https://bookdown.org/home/)网站上寻找。
5. [RStudio](https://www.rstudio.com/)。许多用户初次见到标准的R语言界面时都会觉得它太简陋了，并且代码编写的过程并不友好，需要记住大量的命令和函数。RStudio作为R语言的一个好用的集成开发环境（Integrated Development Environment，简称IDE），在编写R代码时，它能够自动填补以及快速显示函数定义，并且能够随时对代码进行调试。此外，RStudio也是免费的并且支持Windows、MacOS和Linux等不同的操作系统。关于RStudio的更多内容请见第1.3节。

> :pushpin:许多R语言大佬习惯将自己编写的书籍免费发布在网上，这给初学者提供了极大的便利。耳熟能详的R技术大牛[Hadley Wickman](http://hadley.nz/)的代表作[*R for Data Science*](https://r4ds.had.co.nz/)、[*ggplot2: Elegant Graphics for Data Analysis*](https://ggplot2-book.org/index.html)和[*Advanced R*](http://adv-r.hadley.nz/) 均可免费在网上阅读，而国内则有北京大学李东风老师的[《R语言教程》](https://www.math.pku.edu.cn/teachers/lidf/docs/Rbook/html/_Rbook/index.html)。

> :loudspeaker:R语言初学者要养成收藏网址的好习惯，无论是关于问题的解答还是有趣的学习资源，把它们及时添加到收藏夹是非常明智的做法。否则当你需要再次寻找这些内容时，可能会比较麻烦。此外，在google搜索引擎无法使用的情况下，推荐使用[bing](https://cn.bing.com/?FORM=BEHPTB)搜索引擎，并且英文搜索的结果通常会比中文结果更加详实丰富。

金无足赤，白璧微瑕。尽管R语言具有众多的优点，但这并不能掩盖其自身存在的劣势。第一，R语言需要通过编写代码的方式来实现相关功能，这对那些不具编程经验和对统计方法掌握得不是很好的初学者是一大挑战，因此其学习曲线是比较陡峭的。第二，尽管R语言及其扩展包的更新是对当前环境的完善补充，但过快的更新有时会造成许多功能和学习资源跟不上版本的更迭，这就要求R用户必须定期更新，如果不更新会出现很多问题。

[^4]:详情请查看*An Introduction to R*一书：https://cran.r-project.org/doc/manuals/r-release/R-intro.pdf

### 1.1.4 R语言的获取与安装

获取和安装R语言是非常容易的，具体步骤如下：

第一步：打开R语言官方网站（https://www.r-project.org/），点击`download R`；

第二步：在弹出的镜像页面选择合适的镜像入口。截至2021年4月份，中国大陆共有10个镜像入口，你可以选择China下离你最近的一个镜像即可；

第三步：在弹出的下载页面根据自己电脑的操作系统选择安装程序，这里我们选择的是Windows系统；

第四步：在下载页面的子目录下有四类不同的安装文件，点击base版本中的`install R for the first time`进行下载；

第五步：双击下载的R-4.0.5-win.exe，进入安装界面，建议选择默认安装，依次点击`Next >`按钮即可完成。为避免安装出现问题，所有的路径最好都采用英文。

<center>
    <figure>
    <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210411005715746.png", width="600"/>
    </figure>
    <span id="1-website">第一步：R语言官方网站</span>
</center>

<center>
    <figure>
    <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210411005350779.png", width="600"/>
    </figure>
    <span id="1-mirrors">第二步：选择合适的镜像入口</span>
</center>

<center>
    <figure>
    <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210411074240233.png", width="600"/>
    </figure>
    <span id="1-downloados">第三步：根据操作系统选择</span>
</center>

<center>
    <figure>
    <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210411074354803.png", width="600"/>
    </figure>
    <span id="1-downloadbase">第四步：下载base版本安装文件</span>
</center>

<center>
    <figure>
    <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210413232757715.png", width="250"/>
    <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210413234613177.png", width="400"/>
    </figure>
    <span id="1-downloados">第五步：打开exe文件进行默认安装</span>
</center>


安装完成之后，在开始菜单中就会弹出R应用程序的图标，点击该图标，就同时打开了R语言的图形用户界面和控制台，如[图4](#1-rgui)所示。可以看出，它确实十分简陋。不过请放心，我们后续的工作都是在RStudio中展开的，而不是在R应用程序中。

<center>    
    <figure class="half">    
        <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210410003455675.png" width="750"/>    
    </figure>    
    <span id="1-rgui">图4：Windows 10系统中的R语言界面
    </span>
</center>

> :pushpin:CRAN是Comprehensive R Archive Network的首字母简写形式，是拥有同一资料包括R的发布版本、包、文档和源代码的网络合集。CRAN Mirrors镜像站就是把一个网站资源的副本放在镜像服务器上，也就是说登录不同的镜像网站都跟登录主网站一样。而选择一个离我们近的镜像主要是为了下载的快！当然如果主网站不小心坏掉，镜像网站也是一个很好的后备。
>

> :pencil:试着在R语言的命令窗口输入以下代码：`print("Hello, world")`，然后按回车键查看结果。恭喜你编写了R语言的第一行命令，后面的学习之旅会更加精彩！

## 1.2 RStudio简介

作为一个优秀的R语言集成开发环境（IDE），RStudio通过添加一些方便的特性和工具从而能够充分发挥R语言的优势并有效提高使用效率。所谓集成开发环境，就是把你做开发工作所需要的代码编辑器、编译器、调试器等工具都集成在一个界面环境下，方便同时使用。打个比方，如果说R语言像汽车的发动机，那么RStudio就像汽车的仪表盘。使用速度表、后视镜和导航系统能够使驾驶变得更轻松，而使用RStudio也会让使用R的过程的变得更容易。

RStudio可以免费在其[官网](https://www.rstudio.com/)（https://www.rstudio.com/）下载安装。同样地，我们建议采用默认安装并且路径不要出现中文，并且在安装RStudio之前要确保已经安装了R。

### 1.2.1 RStudio的界面

安装完成后，打开RStudio的主界面，如[图5](#1-rstudio-interface)所示。可以看出，在菜单栏和工具栏下方一共分成了四个工作区域，通过拖动中间的分割线可以自由调整工作区域窗口的大小。

<center>    
    <figure class="half">    
        <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210414212529534.png" width="750"/>    
    </figure>    
    <span id="1-rstudio-interface">图5：Windows 10系统中的RStudio语言界面</span>
</center>

A区域是Console区，也被称为控制台，它和RGui编辑器的界面（[图4](#1-rgui)）差不多。这里可以写代码，也可以显示代码运行的过程和结果。但是我们并不建议在这个窗口编写代码，一方面是因为写好的代码不方便保存，二是如果不小心写错代码，就得重新写。该区域上方会显示当前的工作路径为`D:/RProjects/R-book`，点击旁边的箭头则显示当前路径中的文件，右边的<img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210414230253242.png" alt="image-20210414230253242" style="zoom: 50%;" />按钮则用来清空显示，快捷键`Ctrl + L`也可以快速实现这一操作。

B区域是代码编辑区。刚启动RStudio时可能会不显示这个区域，而是A区域占据了整个B区域，可以通过依次点击菜单栏的`File` → `New File` → `R Script`来创建新的代码文件，也可以利用快捷键`Ctrl + Shift + N`。写好代码后，选中代码或把光标停留着某行，点击右边<img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210414225527118.png" alt="image-20210414225527118" style="zoom: 67%;" />图标或快捷键`Ctrl + Enter`来运行这行代码，其结果会在A区域中显示。在代码编写过程中，请及时保存。

C区域是画图安包求助台。Plots界面显示绘制好的图形，可以对其缩放并导出，不仅可以导出为图片格式文件，还可以导出为PDF文件或粘贴到剪切板上。Packages界面显示已经安装的R包的名称、描述和版本信息，打勾则代表该包已经被加载到当前环境中，同时也可以通过点击<img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210414231046633.png" alt="image-20210414231046633" style="zoom: 55%;" />或<img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210414231215334.png" alt="image-20210414231215334" style="zoom:55%;" />来安装或升级R包。Help界面可以很方便地搜索关键词并显示帮助文档。Tutorial界面提示初学者通过安装**learnr**包来学习RStudio教程。Viewer界面用来显示本地网页文件，用得比较少。

D区域是工作空间展示区。Environment界面用来记录代码运行过程中生成的各种对象，包括数据、数值、函数等。History界面显示所有在Console区内代码执行地历史记录，可以将其保存下来，也可以将选中的部分发送到Console区（<img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210414232730915.png" alt="image-20210414232730915" style="zoom:60%;" />）或代码编辑区（<img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210414232912126.png" alt="image-20210414232912126" style="zoom:60%;" />）。Files界面显示工作路径下的所有文件，并且可以对其进行删除或重命名。Connections界面显示连接的外部数据库，用得非常少。

### 1.2.2 RStudio的设置

RStudio安装好之后，我们需要进行一些设置从而使后续的使用更加方便且更具个性化，点击菜单栏的`Tools` → `Global Options`便可以打开设置选项面板（见[图6](#1-rstudio-setting)），从左侧的菜单栏可以看出RStudio可以对代码、界面、拼写等许多内容进行设置。对于初学者来说，常见的设置包括了切换R版本，自定义界面样式，调整窗口布局、设定R包安装镜像以及修改代码编译格式等。

<center>    
    <figure class="half">    
        <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210416113231133.png" width="500"/>    
    </figure>    
    <span id="1-rstudio-setting">图6：RStudio的常规设置选项</span>
</center>

**切换R版本**：R允许一台电脑上同时安装多个不同的版本，通过RStudio可以很方便在各个R版本间进行切换。在打开的选项面板（[图6](#1-rstudio-setting)）下，点击左侧的`General`，在`R version`的下拉框中选择合适的R版本，重新启动RStudio即可切换到相应版本的R。需要注意的是，下拉框中出现的R版本必须提前已经安装到你的电脑上。

**自定义界面样式**：RStudio的默认界面是白色的，但正如[图5](#1-rstudio-interface)所示，我们可以将其修改为自己喜欢的主题颜色。点击左侧的`Appearance`，可以对`RStudio theme`（RStudio主题），`Zoom`（窗口缩放比例），`Editor font`（字体），`Editor font size`（字符大小）以及`Editor theme`（编辑主题）进行个性化设置（[图7](#1-rstudio-appearance)）。

<center>    
    <figure class="half">    
        <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210416115005085.png" width="500"/>    
    </figure>    
    <span id="1-rstudio-appearance">图7：RStudio的界面样式的修改</span>
</center>

**调整工作窗口布局**：RStudio主界面的四个工作区域窗口除了可以自由调整大小之外，还可以调整各自的显示位置及子标签内容。点击左侧的`Pane Layout`，在右侧四个窗口的上方点击下拉按钮，即可将调整这四个工作区域的窗口布局。通过勾选`√`便可以将多个内容显示在同一个工作区域的标签页中（[图8](#1-rstudio-panelayout)）。

<center>    
    <figure class="half">    
        <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210416120410849.png" width="500"/>    
    </figure>    
    <span id="1-rstudio-panelayout">图8：RStudio的窗口布局调整</span>
</center>

**指定R包安装镜像**：RStudio默认从CRAN主网站下载R包，有时会由于网速慢的原因导致安装失败，因此需要设置合适的镜像网站。在`Packages`选项中，点击`change`打开`Primary CRAN repository`的下拉框，选择离自己最近的镜像作为R包的安装来源。当然也可以在下方的`secondary repositorie`s中可以添加备用的镜像网址（[图9](#1-rstudio-packages)）。

<center>    
    <figure class="half">    
        <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210416121438091.png" width="500"/>    
    </figure>    
    <span id="1-rstudio-packages">图9：设置R包的安装镜像</span>
</center>

**修改代码编译格式**：打开别人编写的代码时，里面的中文注释有时候会出现乱码，修改代码编译格式是解决这类问题的办法之一。在`Code`选项中，点击上方的`Saving`，然后将默认的文本编译格式修改为`UTF-8`即可（[图10](#1-rstudio-code)）。

<center>    
    <figure class="half">    
        <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210416123801545.png" width="500"/>    
    </figure>    
    <span id="1-rstudio-code">图10：修改代码默认的编译格式</span>
</center>

安装好R和RStudio之后，我们便可以开展一些基础的数据分析工作。但如果想充分发挥R的强大功能，那么必须通过安装和调用R包来实现。接下来第1.3节我们将对R包展开具体讲解。

## 1.3 R包简介

### 1.3.1 R包是什么？

所谓R包，就是一个把R函数、数据、预编译代码以一种定义完善的格式组织在一起的集合，通过提供额外的函数、数据和文档来扩展R的功能（朱雪宁 等，[2018](https://book.douban.com/subject/30395816/)；Chester Ismay and Albert Y. Kim，[2021](https://moderndive.netlify.app/index.html)）。R包按照其来源可以划分为基础的标准包和捐献的扩展包两大类。基础的标准包是R语言在安装时自动装入的一系列默认包（例如**base**, **datasets**, **stats**, **methods**, **graphics**, **utils**等），这些包是R源代码的重要组成部分，提供了允许R工作的基本函数、数据集、统计方法和图形工具；捐献的扩展包则是由R社区用户开发的可在网上免费下载的包，它们或可以实现某种特定的统计方法，或提供某类数据或硬件的访问接口，或作为教学的补充材料。当然，你也可以根据自身工作需要创建自己的R包，通常包括函数、帮助文档和示例数据等基础内容。

R包和R语言之间的关系是什么样呢？打个比方，我们在上一节安装的R语言程序就像是你手中的一台智能手机，而R包就是安装在这台手机上的各类应用软件（大家俗称的APP）。当你在第一次使用R时，它具备标准包提供的一些基础功能，但并不包含所有的功能，如果你需要更多更厉害的拓展功能，就需要安装扩展包来实现。这就好比你的新手机可以拍照，但拍照效果无法满足你的审美，因此你需要从应用商店中下载一些拍照和美颜软件从而拍出更好看的照片。

### 1.2.2 R包的安装与使用

在安装R包之前，我们首先需要寻找可用的并选择好用的R包。最常用的方法就是通过网络搜索，从而确定哪些包符合自己的需求，还可以通过[CRAN任务视图](https://cran.r-project.org/web/views/)网站（https://cran.r-project.org/web/views/）进行查找，该网站按照不同任务主题将包进行了归类，可以从中寻找与自己需求相近的R包。确定好需要安装的R包之后，接下来就可以开始安装了。

手机APP可以轻松地在应用商店中找到，那么R包从哪儿下载安装呢？一般来说，R包的安装有两种渠道：一种是通过官方的CRAN服务器安装，这是最常见的R扩展包来源；另一种则是从其他渠道下载安装，常见的有Github，Git，Bioconductor等项目库、包含安装包的网址或拷贝到本地的安装包等。下面以**ggplot2**包为例演示R包的安装过程。

**方法一**：打开[图5](#1-rstudio-interface)右上方C工作区域的`Packages`标签页，点击下方的`Install`，然后在打开的窗口中的`Packages (separate multiple with space or comma):`下方一栏中输入要安装的包的名称（此处为`ggplot2`），最后点击右下角的`Install`按钮（[图11](#1-rstudio-pkginstall)）。

<center>    
    <figure class="half">    
        <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210416193722382.png" width="400"/>    
    </figure>    
    <span id="1-rstudio-pkginstall">图11：RStudio中R包的安装方法之一</span>
</center>

**方法二**：在RStudio的控制台窗口输入`install.packages("ggplot2")`，然后按回车键即可完成**ggplot2**包的安装。需要注意的是，代码中的R包名称必须要用英文引号括起来。

**方法三**：假如你需要从Github网站上下载安装R包，首先利用上述两种方法安装**devtools**包，然后再通过其中的`install_github`命令安装，以**ggplot2**包为例，代码如下所示：

```R
install.packages("devtools") # 首先安装devtools包
devtools::install_github("tidyverse/ggplot2") #然后安装ggplot2包
```

由于发布到Github网站上的R包可能存在重名的现象，因此用上述代码安装R包时需要在前面加上它的作者在Github上的用户名，此处的用户名为`tidyverse`。

当需要对R包进行更新时，可以通过以下两种方法实现：一是输入命令`update.packages()`，二是点击[图11](#1-rstudio-pkginstall)中`Install`旁边的`Update`按钮。

> :pencil:尝试采用上面的方法安装**tidyverse**包和**sf**包，并比较这三种方法的优劣。另外，从网上搜索如何一次安装多个R包。

R包安装完成之后，并不能直接使用。只有当它被加载到当前的工作环境中，它包含的命令和数据集才可以被访问或使用。这种做法的目的有两个，一是提高R的工作效率，因为加载所有的R包会消耗大量内存并且增加搜索时间，二是避免出现冲突，因为不同R包可能存在命令或数据集名称重复的现象。加载R包的方式非常简单，仍然以**ggplot2**包为例，使用命令`library(ggplot2)`或者在`Packages`标签页的R包列表中勾选**ggplot2**包（[图12](#1-rstudio-pkglibrary)）都可以完成加载。

<center>    
    <figure class="half">    
        <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210416210442990.png" width="500"/>    
    </figure>    
    <span id="1-rstudio-pkglibrary">图12：RStudio中R包的加载方法之一</span>
</center>

对于初学者而言，R包中的命令及参数如何使用是最令人头疼的问题。除了网络搜索之外，主要的方法是学会查看帮助文档。对于R包而言（仍以**ggplot2**包为例），输入命令`help(package = "ggplot2")`，就可以打开**ggplot2**包的帮助文档界面，里面包含了对该包的整体描述、使用指南等文档，也包含了所含的函数列表，点击名称即可查看该函数的具体用法（[图13](#1-rstudio-pkghelp)）。对于函数而言（以`dim`函数为例），输入命令`help(dim)`，打开`dim`函数的帮助文档，其中的`Description`和`Usage`描述了函数的基本功能和用法，`Arguments`则给出了每个参数的具体含义和用法，最后面的`Examples`可以粘贴到编辑器中运行，从而加深对该函数的理解和体会（[图14](#1-rstudio-fcthelp)）。此外，使用命令`?dim`也可以实现上述的查找，其结果和`help(dim)`是一致的。

<center>    
    <figure class="half">    
        <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210416214741210.png" width="500"/>    
    </figure>    
    <span id="1-rstudio-pkghelp">图13：ggplot2包的帮助文档界面</span>
</center>

<center>    
    <figure class="half">    
        <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210416223503734.png" width="500"/>    
    </figure>    
    <span id="1-rstudio-fcthelp">图14：dim函数的帮助文档</span>
</center>

> :pencil:查看**tidyverse**包和**sf**包的帮助文档，结合网络搜索结果来进一步理解这两个包的主要功能。查看这两个R包中常用函数（如`filter()`和`st_crs()`）的帮助文档，并将`Examples`中的结果复现出来。分别运行`?dim`和`??dim`，比较两者的查找结果有何区别。


## 1.4 更多补充

通过前面三节的介绍，我们对R语言、RStudio和R包有了一定的了解。在此基础上，许多R初学者便迫不及待开始编写自己的R代码。然而在这个过程中，我们通常会遇到一些问题，例如为什么编写代码的速度这么慢？为什么代码一团乱麻，让人没耐心看完？如何寻找合适的学习资源？等等。这些问题分别涉及到快捷键的使用、代码编写规范以及寻找学习资源等三方面内容。在正式进入下一章的学习之前，对这三个问题的解答将会大有裨益，可以避免R初学者走不必要的弯路。

### 1.4.1 RStudio常用快捷键

RStudio是编写和运行R代码的主战场，掌握RStudio的常用快捷键能够大大提高代码编写的速度，真正做到事半功倍。[表1](#1-rstudio-hotkeys)给出了RStudio中常用的快捷键及其功能，后面的备注说明了这些快捷键的应用场景，根据其重要程度和使用频率评为三个等级，星数（:star:）越多表示该快捷键越重要或越经常被用到，建议将这些快捷键都背记下来。

<center><span id="1-rstudio-hotkeys">表1：RStudio常用快捷键</span></center>

| 功能                       | Windows快捷键    | 备注                         |        等级        |
| -------------------------- | ---------------- | :--------------------------- | :----------------: |
| **控制台（Console）**      |                  |                              |                    |
| 清空控制台                 | Ctrl + L         | 清除之前命令的运行结果       |    :star::star:    |
| 定位到某条历史记录         | Ctrl + Up/Down   | 找到之前运行过的命令         |       :star:       |
| **代码编辑区（Source）**   |                  |                              |                    |
| 快速新建脚本               | Ctrl + Shift + N | 修改旧脚本时建议新建脚本     |    :star::star:    |
| 赋值符号（<-）             | Alt + -          | 建议用 <- 而不是 =           | :star::star::star: |
| 管道操作符（%>%）          | Ctrl + Shift + M | **Tidyverse**包工作流中常用  | :star::star::star: |
| 添加/取消注释              | Ctrl + Shift + C | 增强代码的可理解性           | :star::star::star: |
| 插入代码块                 | Ctrl + Shift + R | 将单个任务合并为一个代码块   | :star::star::star: |
| 折叠单个代码块             | Alt + L          | 节省光标下滑时间             |    :star::star:    |
| 展开单个代码块             | Alt + Shift + L  | 回顾该代码块中的代码         |       :star:       |
| 折叠所有代码块             | Alt + O          | 折叠之后类似于代码目录       |    :star::star:    |
| 展开所有代码块             | Alt + Shift + O  | 关注脚本每一行的代码         |    :star::star:    |
| 运行光标所在行或选中的代码 | Ctrl + Enter     | 边写代码边运行，方便修改调整 | :star::star::star: |
| 运行脚本里面的所有代码     | Ctrl + Alt + R   | 快速重现脚本的运行结果       |    :star::star:    |

最后一个关键的快捷键`Alt + Shift + K`会调出RStudio的快捷键面板，里面会详细给出所有的快捷键及其表示的功能，也可以通过点击`Tools` → `Keyboard Shortcuts Help`打开。

除了上述列举的常用的快捷键之外，RStudio官网提供了最为全面快捷的使用方法，详情可以查看RStudio IDE: Cheet Sheet https://github.com/rstudio/cheatsheets/raw/master/rstudio-ide.pdf。


### 1.4.2 代码编写规范

R代码是由命令、参数、对象、符号等一系列要素组成的。虽然代码是否整洁美观并不影响其运行结果，但是规范的R代码会让人耳目一新、眼前一亮，更容易被理解、分享和验证，因此R初学者要从一开始就养成编写规范的、可读性强的代码的好习惯。本节主要介绍初学者在数据分析过程中常用到的一些代码编写规范。

1. **文件名称**：文件命名尽量采用英文，且具有一定的含义（如英文单词或汉语拼音等），可以使用`_`或`-`连接，避免使用汉字、空格或其他特殊符号，如果同时多个文件最好加上序号，如`fit_models.R`或`01_explore.R`。

2. **对象名称**：变量名称优先采用英文名词的小写格式，单词之间用`.`连接，如`avg.clicks`，函数名称则优先采用首字母大写的英文动词，不要使用`.`，如`CalculateAvgClicks`，要尽量避免与R中已有的名称重复。

3. **空格的使用**：

   - 逗号：一定要在逗号后而不是逗号前使用空格，如`x[, 1]`；

   - 圆括号：常规函数命令的圆括号前后不加空格，如`mean(x, na.rm = TRUE)`，在`if`，`for`和`while`命令后的圆括号都要加上空格，如`if (debug) {}`，在function参数的圆括号后面添加一个空格，如`function(x) {}`；

   - 双重花括号：内部对象的前后都要有空格来强调其特殊性，如；

   - ```R
     max_by <- function(data, var, by) {
       data %>%
         group_by({{ by }}) %>%
         summarise(maximum = max({{ var }}, na.rm = TRUE))
     }
     ```

   - 二进制运算符：`==`, `+`, `-`, `<-`等符号前后都要有空格，如`height <- (feet * 12) + inches`;

   - 不用空格特殊情况： `::`, `:::`, `$`, `@`, `[`, `[[`, `^`, `:`和`?`等高优先级的符号前后不用空格，

4. **句型语法**：

   - 每行代码最长不超过80个字符；
   - 使用`<-`进行赋值, 不用`=`赋值，如`x <- 5`；
   - 不要用分号将多个命令放置于一行；
   - 善于使用注释，整行注释以`#`后接一个空格开始，行内短注释在代码后加两个空格再接`#`加一个空格。

上述列举的代码编写规范是R初学者最常遇到的情景，除此之外，在R包的开发过程中及其他场景也存在许多有用的规范，可以使你编写的代码整洁可读，更多的信息请参考[谷歌R语言用户社区规范](https://google.github.io/styleguide/Rguide.html)和[R风格指南](https://style.tidyverse.org/)。此外，**formatR**包可以对R代码进行自动化排版，自动设置空格、缩进、换行等代码格式，让代码看起来更友好。

### 1.4.3 其他注意事项

**入门书籍选择**：前面提到，R语言的学习曲线十分陡峭，并不是所有的书籍都适合初学者，对于没有编程经验的人来说，选择门槛较低的书籍可以帮助他们迅速入门R语言并建立学习的自信心。入门书籍中要尽量避免带有Programming（编程）字眼或统计推导知识较多的书籍，如《[R语言编程艺术](https://book.douban.com/subject/24699632/)》和[*The R book*](https://onlinelibrary.wiley.com/doi/book/10.1002/9781118448908)等，这两类书籍通常是计算机和专业统计背景的人编写的，可以作为后期提高的书籍，但在前期难度太大且会分散许多精力。相比之下，《学习R》和《R语言实战》是两本比较适合初学者的入门书籍，对于其中的基础内容要熟练掌握，多加练习。

**获取学习资源**：在R学习过程中会经常遇到各种各样的问题，优质高效的学习资源能够帮助初学者快速掌握R语言。点击RStudio菜单栏的`Help` → `R Help`，在帮助窗口中会列出R和RStudio的一系列有用的学习资源，点击相应的链接即可打开这些学习资源（[图15](#1-rstudio-help)）。此外，在R代码运行遭遇bug或者想要寻找新功能的时候，网络搜索通常是不二之选，相比于中文，英文查询的资料结果通常更加丰富多样，包含了优质回答、开放书籍等内容，因此具备一定的英语基础对于学习R十分有用。

<center>    
    <figure class="half">    
        <img src="https://gitee.com/dolphinxi/picbed/raw/master/image-20210420140458733.png" width="500"/>    
    </figure>    
    <span id="1-rstudio-help">图15：RStudio自带的学习资源</span>
</center>

**其他学习建议**：首先，学会使用RStudio的新建项目功能将极大地提高你管理文件的能力，通过点击菜单栏的`File` → `New Project`创建一个新的项目，将用到的数据、脚本和结果保存在这个文件夹中。下一次打开该项目时，其所在的文件夹就会被默认地设置为工作路径，避免文件导入导出时频繁地更改工作路径，让你能够更加专注于数据分析。其次，养成记录笔记的好习惯，可以采用CSDN博客或微信公众号来记录学习的历程，按照不同的标签（R包的学习、bug的解决、统计知识基础等）分类汇总，有助于建立自己的知识树和技能树。最后，R的学习是个日积月累的过程，除了学习资料中的示例外，“干中学”是帮助你理解代码和提升自信的最有效的途径。尽管大部分的R代码只需要复制粘贴修改就能够满足自己的使用需求，但是前提是你要对代码的功能及其中的命令或参数足够熟悉。因此，在学习初期切勿眼高手低，代码一定要亲自动手敲键盘！代码一定要亲自动手敲键盘！代码一定要亲自动手敲键盘！（重要的事情说三遍）。







