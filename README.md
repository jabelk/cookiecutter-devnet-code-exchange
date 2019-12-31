# Cookie cutter Template for DevNet Code Exchange Projects

A template for DevNet Code Exchange projects using [cookiecutter](https://github.com/audreyr/cookiecutter)

# How to use this template

```
$ pip install cookiecutter
$ cookiecutter https://github.com/jabelk/cookiecutter-devnet-code-exchange.git
```

You will be asked about your basic info (name, project name, description, etc.). This info will be used in your new project.

> Note: This template assumes the BSD 3-Clause License, you can change it be other licenses afterwards if that is not what you want.


## Example 
```bash
use-cases$ cookiecutter -h
Usage: cookiecutter [OPTIONS] TEMPLATE [EXTRA_CONTEXT]...

  Create a project from a Cookiecutter project template (TEMPLATE).

  Cookiecutter is free and open source software, developed and managed by
  volunteers. If you would like to help out or fund the project, please get
  in touch at https://github.com/audreyr/cookiecutter.

Options:
  -V, --version              Show the version and exit.
  --no-input                 Do not prompt for parameters and only use
                             cookiecutter.json file content
  -c, --checkout TEXT        branch, tag or commit to checkout after git clone
  -v, --verbose              Print debug information
  --replay                   Do not prompt for parameters and only use
                             information entered previously
  -f, --overwrite-if-exists  Overwrite the contents of the output directory if
                             it already exists
  -o, --output-dir PATH      Where to output the generated project dir into
  --config-file PATH         User configuration file
  --default-config           Do not load a config file. Use the defaults
                             instead
  --debug-file PATH          File to be used as a stream for DEBUG logging
  -h, --help                 Show this message and exit.
use-cases$ cookiecutter https://github.com/jabelk/cookiecutter-devnet-code-exchange.git
project_name [my-awesome-devnet-code-exchange-project]: my-first-project
project_description [baseline DevNet Code Exchange Project]: New Things to come!
author_name [Your Name Here]: Jason Belk
author_email [youremail@domain.com]: jabelk@cisco.com
use-cases$ tree
.DS_Store                          devnet-code-exchange/              my-first-project/
cookiecutter-devnet-code-exchange/ 
use-cases$ tree my-first-project/
my-first-project/
├── LICENSE
├── NOTICE
└── README.md

0 directories, 3 files
use-cases$
```

If it is already downloaded, you can redownload or reuse the existing repo:
```bash
use-cases$ cookiecutter cookiecutter-devnet-code-exchange/
project_name [my-awesome-devnet-code-exchange-project]: my-second-project
project_description [baseline DevNet Code Exchange Project]:
author_name [Your Name Here]:
author_email [youremail@domain.com]:
use-cases$ tree my
my-first-project/  my-second-project/
use-cases$ tree my-second-project/
my-second-project/
├── LICENSE
├── NOTICE
└── README.md

0 directories, 3 files
use-cases$ ls
cookiecutter-devnet-code-exchange		my-second-project
devnet-code-exchange			my-first-project
use-cases$
```