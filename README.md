# A Virtual Machine for Rust Core Development

## Introduction

This is a machine image designed for rust language core development. It's heavily 
inspired by the rails-dev-box project.

## Requirements 

* [VirtualBox](https://www.virtualbox.org)

* [Vagrant](http://vagrantup.com)

## How to use

1. Clone the repo on your host machine. 

```bash
git clone git@github.com:estsauver/rust-dev-box.git
```

2. Launch the box. (This will take a while.)

```bash
cd rust-dev-box
vagrant up
```

After the installation, you can ssh into the box. 

## Recommended Workflow

Rust will be installed in the ~/dev/rust directory. 

## License

Released uner the MIT License, Copyright 2015 - Earl St Sauver
