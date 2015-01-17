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
git clone $$$REPO_URL HERE$$$
```

2. Launch the box. (This will take a while.)

```bash
cd rust-dev-box
vagrant up
```

After the installation, you can ssh into the box. 

## Recommended Workflow

After running vagrant up, the contents of the rust-dev-box
directory will be available in the guest at `/vagrant`. If you clone
your personal fork into the rust-dev-box, then you can edit it the editor
of your choice on the host and run the tests inside the vm.

## License

Released uner the MIT License, Copyright 2015 - Earl St Sauver
