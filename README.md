# secPassword

<div align="center">
  <img src="/img/sec-logo.png" width=750px>
</div>

Bash script that allows to create random passwords with high entropy, depending on the definition of certain assigned parameters 

---

## Install tool

* Download the repository to your system

```shell
sudo git -C /opt clone https://github.com/iTroxB/secPassword.git
```

* To use the system-level tool as an executable from a relative path, it is recommended to create a symbolic link to the /usr/bin directory from your repository directory.

```shell
sudo chmod +x /opt/secPassword/secPassword.sh
sudo ln -s /opt/secPassword/secPassword.sh /usr/bin/secPassword
```

* To know the options and parameters of the tool run the help menu with the flag `-h` or `--help`.

```shell
secPassoword -h
```

```shell
secPassoword --help
```

<div align="center">
  <img src="/img/sec-help.png" width=750px>
</div>

---

## Use tool

<div align="center">
  <img src="/img/sec-init.png" width=750px>
</div>

- Always declare the length of the password to be created with the -l parameter, and at least one of the parameters assigned to the type of characters used.

<div align="center">
  <img src="/img/sec-l.png" width=750px>
</div>

<div align="center">
  <img src="/img/sec-lm.png" width=750px>
</div>

- Password created with all parameters used

<div align="center">
  <img src="/img/sec-lMmns.png" width=750px>
</div>
