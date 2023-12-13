## Installation

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

**Note**: auto-completion works when you create a Python package and run it with `--install-completion` or when you use <a href="https://typer.tiangolo.com/typer-cli/" class="internal-link" target="_blank">Typer CLI</a>.


