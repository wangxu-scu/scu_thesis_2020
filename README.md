<div align="center"><img style="display:inline-block" width='150' src="./assets/icon.png"/><p>
    <span style="font-size: 14px">Version: 2020.03.13</span><br>
    <span>"2020年四川大学研究生学业论文LaTex模版"</span><br>
    <span style="font-size: 12px;color= #95dafc">-- Modified by <a>Kevin T. Lee</a> --</span>
    </p>
   <a href="./License"><img alt="GPL" src="https://img.shields.io/badge/LICENSE%20-GPL-green.svg?longCache=true&style=for-the-badge"></a>
        <a href="http://lidengju.com"><img alt="Code" src="https://img.shields.io/badge/Code%20with-Love-red.svg?longCache=true&style=for-the-badge"></a>
   <a href="http://lidengju.com"><img alt="Code" src="https://img.shields.io/badge/%E6%AD%A6%E6%B1%89%0A-%E5%8A%A0%E6%B2%B9-red.svg?longCache=true&style=for-the-badge"></a>
    <a href="https://github.com/kevinleeex/scu_thesis_2020"><img alt="Version" src="https://img.shields.io/badge/Version-2020.03.13-blue.svg?longCache=true&style=for-the-badge"></a>
</div>


# 四川大学2020研究生学业论文LaTex模版

根据学院给的2020版《研究生学位论文规范写作指南》Word模版需求([导出PDF](./Reference%20Document/1-3%20《研究生学位论文规范写作指南》.pdf))，并基于fork的旧版库样式，改写了模版。

SCU graduate thesis latex template.

> 独立的模版样式文件，[scu_thesis_template](https://github.com/kevinleeex/scu_thesis_template)，可用于替换```./Template```目录用于更新样式。

## :warning:NOTICE

现在发现几处给出范例与描述不一致，已根据理解修改，如下：

- 页眉说明为五号字，范例为小五，修改为**小五**。
- 一些标题描述间隔一个汉字符，范例为一个空格符，修改为**一个汉字符**。
- 封面页校名标题没有居中，修改为**居中**。
- 描述中公式居中，范例为右对齐，添加右对齐功能，默认**居中**。
- 描述中图和表题注都为宋体加粗，范例的表为黑体，修改为**宋体加粗**
- 没有保留封面等内容的说明内容。
- 部分内容由于排版软件的关系有些微差别。

> 如您发现更多问题请您提交ISSUES，或PR。
>
> **免责声明：本项目开源用于格式参考，本模版的作者和贡献者不承担任何人使用该模版所引发的任何问题(如格式审查等)。**
>
> 考虑之前的fork的项目与原项目差异已较大，且不易被需要的人搜索到，所以将项目独立出来。

## Features

- [x] 🍞 通过配置项自动生成不同类型的论文格式，你专注内容就好
- [x] 🍔 「像素级」复刻原Word模版
- [x] 🧀  通过```\incite``` 来进行行内引用
- [x] 🍟 ```\bicaption```图片双语题注示例
- [x] 🍕 ```\cdash```公式说明的破折号
- [x] 🌮 ```\cref```智能参考
- [x] 🥘 ```\tabincell```多行单元格

## Options

| 参数         | 说明                                                 |
| ------------ | ---------------------------------------------------- |
| professional | 专业学位                                             |
| academic     | 学术学位                                             |
| master       | 硕士                                                 |
| docter       | 博士                                                 |
| approval     | 送审版本，不生成声明和致谢                           |
| color        | 红色川大logo，默认为黑色                             |

## Release Notes

See [Releases](https://github.com/kevinleeex/scu_thesis_2020/releases)

- [2020-02-19] 将Template作为[子模块](https://github.com/kevinleeex/scu_thesis_template)方便样式的后续更新。 
- [2020-03-13] **推荐**[scu_thesis_2020_03_13](https://github.com/kevinleeex/scu_thesis_2020/releases/download/v2020.03.13/scu_thesis_2020_03_13.zip)点击下载。
## Previews
![image-20200301232656767](assets/image-20200301232656767.png)

双语图片标题示例：

![image-20200301232622548](assets/image-20200301232622548.png)

三线表示例：

![image-20200301232947151](assets/image-20200301232947151.png)

## Getting Started

### Prerequisites

The following softwares you should installed before build the project.

- TexLive
- MacTex(on mac)
- Visual Studio Code (optional) with LaTex workshop plugin

### Installation

Clone the project.

```bash
cd path-to-dir
git clone https://github.com/kevinleeex/scu_thesis_2020.git
cd scu_thesis_2020
git submodule init
code scu_thesis_2020
```

**后续通过```git submodule update --remote```命令 更新样式子模块到最新版本。**

### Usages

Open and edit the ```MainBody.tex```

```shell
% 设置文档属性
% 参数说明
% professional: 专业学位
% academic: 学术学位
% master: 硕士
% doctor: 博士
% approval: 送审版本，将不生成声明
% color: 红色川大logo
% 打开MainBody.tex根据需要填入
\documentclass[professional,master]{./Template/scuthesis2020}

% 在./Chapter/ 文件夹中写作，在MainBody.tex中包含
% 在./ReferenceDocument/ 文件夹中，存放用于参考的文献
% 在./ReferenceBase.bib 文件中存放bibTex引用
```

Use **xelatex** compile the LaTex file with the recipe of ```xe->bib->xe->xe``` .

## Powered By

- [cuiao's template](https://github.com/cuiao/SCU_ThesisDissertation_LaTeXTemplate)

I would like to extend my sincere gratitude to the authors and contributors of the open source libraries above.

## Support me

If this project helps you, you can support me to do better.  
<a href="https://paypal.me/kevinleeex"><img alt="Coffee" src="https://img.shields.io/badge/PayPal_me_a-Coffee-7A501E.svg?longCache=true&style=for-the-badge"></a>

Or click <a href="http://lidengju.com/donate">Donete me</a> with Wechat or Alipay

And Star/ISSUE/PR are welcome.

## License

Copyright © 2020 Modified by [Kevin T. Lee](http://lidengju.com). All rights reserved. 

The project is licensed under the GPL license. See [LICENSE](./License/) for more details.
