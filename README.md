# Ansible Examples

## Installation

1. Install Virtualenv:
```
$ pip install --upgrade virtualenv
```

2. Activate it:
```
$ source env/bin/activate
```

3. Install Ansible and it's dependencies:
```
$ pip3 install ansible
```

4. Install [Vagrant](https://www.vagrantup.com) and [VirtualBox](https://www.virtualbox.org)


## Usage

1. Launch Vagrant:
```
$ vagrant up
```

2. Execute Ansible test:
```
$ ansible vagrant -i inventory -m ping
```

3. Install Ansible module from external repo:
```
$ ansible-galaxy install geerlingguy.nginx
```

4. Apply a Role:
```
$ ansible-playbook -i inventory nginx.yml -b
```

5. Test the installation:
```
$ ansible vagrant -i inventory -a "hostname -I"
27.0.0.1 | SUCCESS | rc=0 >>
10.0.2.15 10.0.0.10 2601:647:5080:60a0:a00:27ff:fe31:e7d8

http -b 10.0.0.10
<!DOCTYPE html>
<html>
<head>
<title>Welcome to nginx!</title>
<style>
    body {
        width: 35em;
        margin: 0 auto;
        font-family: Tahoma, Verdana, Arial, sans-serif;
    }
</style>
</head>
<body>
<h1>Welcome to nginx!</h1>
<p>If you see this page, the nginx web server is successfully installed and
working. Further configuration is required.</p>

<p>For online documentation and support please refer to
<a href="http://nginx.org/">nginx.org</a>.<br/>
Commercial support is available at
<a href="http://nginx.com/">nginx.com</a>.</p>

<p><em>Thank you for using nginx.</em></p>
</body>
</html>
```
