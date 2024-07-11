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

- Execution on base64-encoded JWT without secret signature

  - **Token**: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYW1lIjoiSm9obiBEb2UifQ.5Hm3bNazVbnK--vsGWMJ_tmZCviy7qL4T16XJLBtQq0
  - **Base64-encode**: ZXlKaGJHY2lPaUpJVXpJMU5pSXNJblI1Y0NJNklrcFhWQ0o5LmV5SnVZVzFsSWpvaVNtOW9iaUJFYjJVaWZRLjVIbTNiTmF6VmJuSy0tdnNHV01KX3RtWkN2aXk3cUw0VDE2WEpMQnRRcTA=

<div align="center">
  <img src="/img/-token1.png" width=900px>
</div>

- Execution on base64-encoded JWT with brute force attack on secret signature "JSON-WEB-TOKEN"

  - **Token**: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYW1lIjoiSm9obiBEb2UifQ.VVrywxLuWdr8seumIsY49n_OL4l_k7xph745wdr9_BM
  - **Base64-encode**: ZXlKaGJHY2lPaUpJVXpJMU5pSXNJblI1Y0NJNklrcFhWQ0o5LmV5SnVZVzFsSWpvaVNtOW9iaUJFYjJVaWZRLlZWcnl3eEx1V2RyOHNldW1Jc1k0OW5fT0w0bF9rN3hwaDc0NXdkcjlfQk0=
 
<div align="center">
  <img src="/img/-token2.png" width=900px>
</div>
