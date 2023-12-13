# Get Started

## 代码高亮

```python
print('hello world!')

class LinkList:

    def __init__(self):
        self.head = Node(None)

    def init_list(self, list_target):
        p = self.head
        for i in list_target:
            p.next = Node(i)
            p = p.next
```

## shell 终端安装效果

<div class="termy">

```console
$ pip install "mkdocs"
---> 100%
Successfully installed mkdocs
```
</div>

## Example

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

!!! failure "这是 failure 类型的提示框"

!!! bug "这是 bug 类型的提示框"

!!! tip "这里是普通提示信息"

