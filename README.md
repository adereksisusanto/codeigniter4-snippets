# Codeigniter 4 Snippets for Vscode

This Extensions provides the Codeigniter 4 snippets

## Requirements

```bash
CodeIgniter Version : 4.1.1
```

## Install

Launch Code's command palette

```bash
ext install codeigniter4-snippets
```

## Avaiable snippets

#### 1. in Views

| Command        | Description                    | Example                                                                                        |
| -------------- | ------------------------------ | ---------------------------------------------------------------------------------------------- |
| ci4_php        | Make <b>php</b>                | `<?php code_here ;?> `                                                                         |
| ci4_php_echo   | Make <b>php echo</b>           | `<?= code_here ;?> `                                                                           |
| ci4_section    | Make <b>section</b>            | `<?= $this->section('code_here') ;?>`                                                          |
| ci4_endsection | Make <b>endSection</b>         | `<?= $this->endSection() ;?>`                                                                  |
| ci4_sectionend | Make <b>section endSection</b> | `<?= $this->section('code_here') ;?>`<br>`<!-- CODE HERE -->`<br>`<?= $this->endSection() ;?>` |

## Contributing

1. Fork it (<https://github.com/adereksisusanto/codeigniter4-snippets/fork>)
2. Create your feature branch (`git checkout -b my-new-snippet`)
3. Commit your changes (`git commit -am 'Add some snippet'`)
4. Push to the branch (`git push origin my-new-snippet`)
5. Create a new Pull Request

Happy coding!

## License

[![GitHub license](https://img.shields.io/github/license/adereksisusanto/codeigniter4-snippets.svg)](https://github.com/adereksisusanto/codeigniter4-snippets)
