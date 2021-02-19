# Codeigniter 4 Snippets for Vscode

This Extensions provides the Codeigniter 4 snippets

## Requirements

```bash
CodeIgniter Version : 4.1.1
```

## Install

Launch Code's command palette

```bash
ext install adereksisusanto.codeigniter4-snippets
```

## Avaiable snippets

#### 1. in Views

| Command           | Description                    | Output                                                                                         |
| ----------------- | ------------------------------ | ---------------------------------------------------------------------------------------------- |
| ci4_endsection    | Make <b>endSection</b>         | `<?= $this->endSection() ;?>`                                                                  |
| ci4_extend        | Make <b>extend</b>             | `<?= $this->extend('code_here') ;?> `                                                          |
| ci4_include       | Make <b>include</b>            | `<?= $this->include('code_here') ;?> `                                                         |
| ci4_php           | Make <b>php</b>                | `<?php code_here ;?> `                                                                         |
| ci4_php_echo      | Make <b>php echo</b>           | `<?= code_here ;?> `                                                                           |
| ci4_rendersection | Make <b>renderSection</b>      | `<?= $this->renderSection('code_here') ;?> `                                                   |
| ci4_section       | Make <b>section</b>            | `<?= $this->section('code_here') ;?>`                                                          |
| ci4_sectionend    | Make <b>section endSection</b> | `<?= $this->section('code_here') ;?>`<br>`<!-- CODE HERE -->`<br>`<?= $this->endSection() ;?>` |

Happy coding!

## License & Download

[![GitHub license](https://img.shields.io/github/license/adereksisusanto/codeigniter4-snippets.svg)](https://github.com/adereksisusanto/codeigniter4-snippets) ![Visual Studio Marketplace Downloads](https://img.shields.io/visual-studio-marketplace/d/adereksisusanto.codeigniter4-snippets)
