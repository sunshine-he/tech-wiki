# Get Started

## 代码高亮展示

```python title="demo.py" linenums="1"
print('hello world!')

class LinkList:  # (1)! 

    def __init__(self):
        self.head = Node(None)

    def init_list(self, list_target): 
        p = self.head
        for i in list_target:
            p.next = Node(i)
            p = p.next
```

1.  这里是一个定义链表的类

## shell 终端安装效果

<div class="termy">

```console
$ pip install "mkdocs"
---> 100%
Successfully installed mkdocs
```
</div>

## 安装示例

### The absolute minimum

* Create a file `main.py` with:

```Python
import typer


def main(name: str):
    print(f"Hello {name}")


if __name__ == "__main__":
    typer.run(main)
```

### Run it

Run your application:

<div class="termy">

```console
// Run your application
$ python main.py

// You get a nice error, you are missing NAME
Usage: main.py [OPTIONS] NAME
Try 'main.py --help' for help.
╭─ Error ───────────────────────────────────────────╮
│ Missing argument 'NAME'.                          │
╰───────────────────────────────────────────────────╯


// You get a --help for free
$ python main.py --help

Usage: main.py [OPTIONS] NAME

╭─ Arguments ───────────────────────────────────────╮
│ *    name      TEXT  [default: None] [required]   |
╰───────────────────────────────────────────────────╯
╭─ Options ─────────────────────────────────────────╮
│ --help          Show this message and exit.       │
╰───────────────────────────────────────────────────╯

// Now pass the NAME argument
$ python main.py Camila

Hello Camila

// It works! 🎉
```

</div>

**Note**: auto-completion works when you create a Python package and run it with `--install-completion` 


## 漂亮的提示信息
!!! note "这是 note 类型的提示框"

!!! success "这是 success 类型的提示框"

!!! warning "这是 warning 类型的提示框"

!!! failure "这是 failure 类型的提示框"

!!! bug "这是 bug 类型的提示框"

!!! tip "这里是普通提示信息"

???+ note "折叠框"

    这里是正文内容

!!! question "问题框"

    请问你有什么问题需要反馈的呢？

## content tabs

!!! example "示例代码"

    === "C"

        ``` c
        #include <stdio.h>

        int main(void) {
        printf("Hello world!\n");
        return 0;
        }
        ```

    === "C++"

        ``` c++
        #include <iostream>

        int main(void) {
        std::cout << "Hello world!" << std::endl;
        return 0;
        }
        ```



## task list

- [x] 写项目代码
- [ ] 户外活动
    * [x] 和朋友聚餐
    * [x] 打球
    * [ ] 唱歌
- [ ] 无聊刷下视频
  

## 文本高亮标识

### Highlighting text

Text can be {--deleted--} and replacement text {++added++}. This can also be
combined into {~~one~>  a single~~} operation. {==Highlighting==} is also
possible {>>and comments can be added inline<<}.

{==

Formatting can also be applied to blocks by putting the opening and closing
tags on separate lines and adding new lines between the tags and the content.

==}

### Text with sub- and superscripts

- H~2~O
- A^T^A
- 2^3^=8 :smile:

## 卡片栅格效果示例

<div class="grid cards" markdown>

-   :material-clock-fast:{ .lg .middle } __Set up in 5 minutes__

    ---

    Install [`mkdocs-material`](#) with [`pip`](#) and get up
    and running in minutes

    [:octicons-arrow-right-24: Getting started](#)

-   :fontawesome-brands-markdown:{ .lg .middle } __It's just Markdown__

    ---

    Focus on your content and generate a responsive and searchable static site

    [:octicons-arrow-right-24: Reference](#)

-   :material-format-font:{ .lg .middle } __Made to measure__

    ---

    Change the colors, fonts, language, icons, logo and more with a few lines

    [:octicons-arrow-right-24: Customization](#)

-   :material-scale-balance:{ .lg .middle }   __Open Source, MIT__
     
    ---

    Material for MkDocs is licensed under MIT and available on [GitHub]

    [:octicons-arrow-right-24: License](#)

</div>


## 图像展示效果

### 图片居中
<figure markdown>
  ![WeChat](assets/images/trustwin1688.jpg){ width="200" }
  <figcaption>图片居中</figcaption>
</figure>

### 图片居左

![WeChat](assets/images/trustwin1688.jpg){ align=left width=150 }
:material-information-outline:{ title="Important information" }
Important: admonitions that use the inline modifiers must be declared prior to the content block you want to place them beside. If there's insufficient space to render the admonition next to the block, the admonition will stretch to the full width of the viewport, e.g., on mobile viewports.<br><br>


## 快捷键
++ctrl+alt+del++





