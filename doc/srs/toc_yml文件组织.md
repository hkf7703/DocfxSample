# tco.yml文件组织
docfx文档需要有个导航栏， 推荐使用toc.yml组织。 本文将介绍toc.yml的一般组织形式。



## 1.数据模型

数据样例如下：

```yml
- name: Topic1
  href: Topic1.md
- name: Topic2
  href: Topic2.md
- name: Topic3
  items:
    - name: Topic2_1
      href: Topic2_1.md
```

> [!NOTE]
> 注意：属性名大小写敏感。
>
> toc是Table of Content的缩写， 一般指目录。

name: 必须的， 指定TOC 项的标题。

href: 可选的，指定TOC 项的导航路径。如果未指定*href*，则*TOC Item*作为其子*TOC Items*的父容器。推荐使用相对路径。

items: 可选的， 指定当前目录项的子目录项。

参考资料：
[Table-Of-Content (TOC) Files](https://dotnet.github.io/docfx/tutorial/intro_toc.html)

[YAML Ain’t Markup Language (YAML™) version 1.2](https://yaml.org/spec/1.2.2/)