# gh-render-markdown

[gh][1] extension to render markdown files as HTML.

[1]: https://cli.github.com/

## Usage

Specify one or more markdown files to generate as arguments to `gh
render-markdown`:

```
gh render-markdown README.md CONTRIBUTING.md
```

Alternatively, STDIN can be used which allows for a few different usage
patterns. For example, you can redirect input:

```
gh render-markdown < README.md
```

Or pipe a command that outputs markdown:

```
echo '# markdown' | gh render-markdown
```

Or pass raw markdown directly via input:

```
gh render-markdown <<< '# markdown'
```

Or manually type a blob of markdown yourself by opening STDIN (press Ctrl-D
when done):

```
gh render-markdown
# markdown
^D
```

## Installation

```
gh extension install itspriddle/gh-render-markdown
```

## Bug Reports

Issues can be reported on GitHub:

<https://github.com/itspriddle/gh-render-markdown/issues>

## License

MIT License - see [`LICENSE`](./LICENSE) in this repo.
