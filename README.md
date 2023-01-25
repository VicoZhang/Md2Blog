# Md2Blog

## 此程序的目的

在使用 Jekyll 编写博客时，发现了如下一些问题：

1. 图片不能正确显示。因为 Jekyll 自动将 _post 下的文件转换到 _site下 year/month/day 目录下，但是如果直接将 Typora 写好的文件复制到 _post 文件夹，不但 .assets 文件夹下的图片无法复制到 Jekyll 下的 img文件夹中，而且 md 文件中的图片引用地址也无法修改。
1. 公式不能正确显示。按照文章：[jekyll下Markdown的填坑技巧](https://eipi10.cn/others/2019/12/07/jekyll-markdown-skills/)  Jekyll 中需要将 $$ 前后各加一个 \n 

由此诞生本程序。程序可以实现：

1. 将 Typora 中写好的 md 文件自动复制到 Jekyll 下的 _post 目录，并按照要求进行重命名。
1. 将 Typora 中的 .assets 文件夹下图片复制到 Jekyll 下的 img 目录，并完成 md 文件里的引用链接更新。
1. 将 Typora 中的公式格式进行修改。

## 使用方法

1. 复制一份 Md2Blog.py 文件到 Jekyll 目录下，完成程序里的一些基础设置。

2. 进入 cmd 中，cd 到 Jekyll 目录下，然后输入：

    ``` 
    python Md2Blog -i=<md文件路径>
    ```

2. 出现`文件处理完成` ，说明程序使用成功。

## 注意

程序主要部分已经注释，如有需要，请自行修改。如有建议，请告知。
