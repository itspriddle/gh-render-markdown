# gh-render-markdown

[gh][1] extension to render Markdown files as HTML.

[1]: https://cli.github.com/

## Usage

Specify one or more Markdown files to generate as arguments to `gh
render-markdown`:

```sh
gh render-markdown README.md CONTRIBUTING.md
```

Alternatively, STDIN can be used which allows for a few different usage
patterns. For example, you can redirect input:

```sh
gh render-markdown < README.md
```

Or pipe a command that outputs Markdown:

```sh
echo '# markdown' | gh render-markdown
```

Or pass raw Markdown directly via input:

```sh
gh render-markdown <<< '# markdown'
```

Or manually type a blob of Markdown yourself by opening STDIN (press Ctrl-D
when done):

```sh
gh render-markdown
# markdown
^D
```

## Installation

```sh
gh extension install itspriddle/gh-render-markdown
```

## Bug Reports

Issues can be reported on GitHub:

<https://github.com/itspriddle/gh-render-markdown/issues>

## License

MIT License - see [`LICENSE`](./LICENSE) in this repository.
