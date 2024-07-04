---
title: "XXXXXXXXXXXX"
date: 2024-06-03
draft: false
description: "用于创建 Blowfish 主题使用指南的模板"
tags: ["content", "example"]
showauthor: true
slug: ""
tags: ["setup", "doc"]

# series: ["部署教程"]
# series_order: 4
---

感谢您愿意为 Blowfish 社区做出贡献。

## 如何开始？
这是一篇模板文章，将解释如何为 Blowfish 的指南部分创建新文章。

## Clone Blowfish 仓库
使用以下命令 clone 此仓库：

```bash
git clone https://github.com/nunocoracao/blowfish.git
```

## 配置您的文档
复制并粘贴您要创建的 `.md` 文档所在的整个文件夹。
使用 `YYYYMM-<英文标题>` 的格式（例如：`200601-tutorial`）命名文档，不允许有空格。

## 徽章

{{< badge >}}
New article!
{{< /badge >}}

## 按钮


{{< button href="#button" target="_self" >}}
Call to action
{{< /button >}}




## 图表

{{< chart >}}
type: 'bar',
data: {
  labels: ['Tomato', 'Blueberry', 'Banana', 'Lime', 'Orange'],
  datasets: [{
    label: '# of votes',
    data: [12, 19, 3, 5, 3],
  }]
}
{{< /chart >}}


## 提交 PR
提交您的 PR ，Blowfish 团队在这里提前感谢您对我们这个项目的贡献。

## 引入github库

{{< github repo="nunocoracao/blowfish" >}}



## 嵌入bilibili视频

{{< bilibili BV1LJ4m1u7uL >}}

## 嵌入youtube视频

{{< youtubeLite id=KLuTLF3x9sA label="Blowfish-tools demo" >}}



## 时间线
{{< timeline >}}

{{< timelineItem icon="github" header="header" badge="Latest" subheader="subheader" >}}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus non magna ex. Donec sollicitudin ut lorem quis lobortis. Nam ac ipsum libero. Sed a ex eget ipsum tincidunt venenatis quis sed nisl. Pellentesque sed urna vel odio consequat tincidunt id ut purus. Nam sollicitudin est sed dui interdum rhoncus. 
{{< /timelineItem >}}


{{< timelineItem icon="code" header="Another Awesome Header" badge="date - present" subheader="Awesome Subheader" >}}
With html code
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
{{< /timelineItem >}}

{{< timelineItem icon="star" header="Shortcodes" badge="AWESOME" >}}
With other shortcodes
{{< gallery >}}
  <img src="gallery/01.jpg" class="grid-w33" />
  <img src="gallery/02.jpg" class="grid-w33" />
  <img src="gallery/03.jpg" class="grid-w33" />
  <img src="gallery/04.jpg" class="grid-w33" />
  <img src="gallery/05.jpg" class="grid-w33" />
  <img src="gallery/06.jpg" class="grid-w33" />
  <img src="gallery/07.jpg" class="grid-w33" />
{{< /gallery >}}
{{< /timelineItem >}}

{{< timelineItem icon="code" header="Another Awesome Header">}}
{{< github repo="nunocoracao/blowfish" >}}
{{< /timelineItem >}}

{{< /timeline >}}
