# Ansible Examples

## Installation

1. Install Virtualenv:
```
pip install --upgrade virtualenv
```

2. Activate it:
```
source env/bin/activate
```

3. Install Ansible and it's dependencies:
```
pip install -r requirements.txt
```

4. Install [Vagrant](https://www.vagrantup.com)


## Usage

1. Launch Vagrant:
```
vagrant up
```

2. Execute Ansible test:
```
ansible vagrant -i inventory -m ping
```

