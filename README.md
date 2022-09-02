yaml2json
=========  

[![Build Status](https://img.shields.io/github/workflow/status/dafu-wu/yaml2json/CI/main)](https://github.com/dafu-wu/yaml2json/actions?query=workflow%3ACI)
[![Crates.io](https://img.shields.io/crates/v/yaml2json)](https://crates.io/crates/yaml2json)

A command-line tool that converts YAML to JSON.


## Installation

### Cargo

```
$ cargo install yaml2json
```

## Usage

Convert YAML on `stdin` to JSON, filtering it through `jq`:

```bash
$ yaml2json <<< 'okay = "ok"' | jq
```

Convert YAML from a file and pretty-print it without `jq`:

```bash
$ yaml2json --pretty ./demo.yaml
```