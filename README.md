# About

Most modern languages can easily be installed via a package manager with no further configuration, however, Golang is a bit different. After installing Golang it is required that you set custom variables in your shell. Depending on your user and shell, your installation may vary. The goal of this script is to identify your user, OS, and default shell to bootstrap your Golang installation.

# Useage

Ansible must be installed on your local machine. Once installed, just clone this repo and run the command below:

`$ ansible-playbook main.yml`

Check that `GOPATH` is set correctly with this command:
```
$ go env GOPATH
/home/user/go
```

Please note that Ansible will still keep your old .bashrc or .zshrc file backed up in your `$HOME` directory in case you want to revert back to your old configuration.


### Todo
* Reload shell when Ansible script is complete
* Add condition for OS.
* Add roles
