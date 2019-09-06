# acg-snapshotalyzer-30000

Demo project to manage AWS EC2 instance snapshots

## About

This project is a demo, and uses boto3 to manage AWS EC2 instance snapshots.

## Configuring

shotty uses the configuration file created by the AWS CLI. e.g.

`aws configure`

## Running

`pipenv run python shotty/shotty.py <command> <subcommand>  <--project=PROJECT>`

*command* is instances, volumes, or snapshots
*subcommand* - dependes on command
*project* is optional



```
docs/
├── Makefile
|
├── build
│   ├── html
│         ├── index.html
|
├── source
│   ├── conf.py
│   ├── connection.rst
│   ├── index.rst
│   ├── message.rst
│   ├── modules.rst
│   └── static
│       ├── architecture.md
│       ├── data-dictionary.md
│       ├── faq.md
│       ├── help.md
│       └── project-structure.md

```
