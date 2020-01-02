# 文档布局

## 初始结构

文档是普通的 `Markdown` 文件, 放到项目目录里. 通常目录以 `docs` 命名, 和 `mkdocs.yml` 配置文件一起放置于项目的顶级目录中.

最简单的目录结构如下:

```
mkdocs.yml
docs/
    index.md
```

默认项目主页是 `index`.

可以创建多个 markdown 文件以创建多页文档:
```
mkdocs.yml
docs/
    index.md
    about.md
    license.md
```
文档目录结构决定着生成的文档的 `URLs` . 如果采用如上目录结构, 生成的 URLs 将会如下所示:
```
/
/about/
/license/
```

你也可以根据需要将 `Markdown` 文件放到多级目录.

```
docs/
    index.md
    user-guide/getting-started.md
    user-guide/configuration-options.md
    license.md
```

多级目录将生成多级 `URLs`, 如下所示:
```
/
/user-guide/getting-started/
/user-guide/configuration-options/
/license/
```

## 如何设置多级目录
