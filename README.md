# Domoticz

This role installs Domoticz Home Automation System and support for OpenZWave can be enabled. The role is used in the vagrant domoticz environment, that can be found in the following repo https://github.com/ZuydUniversity/domoticz-env[https://github.com/ZuydUniversity/domoticz-env]

## Requirements

None.

### Default usage

As default Domoticz is installed and running http on port 8080 and https on port 8081 (not working at the moment) with the default certificate.

## Example Playbook

Install Domoticz with the default settings
```yaml
- hosts: domoticz-servers
  roles:
     - { role: domoticz }
```
After running the playbook, Domoticz can be found for HTTP at http://ipaddress:8080 and HTTPS at https://ipaddress:8081

## Development Requirements

### Create an environment
Create a project folder and a venv folder within:
```
mkdir myproject
cd myproject
python3 -m venv venv
```

On Windows:
```
py -3 -m venv venv
```

If you needed to install virtualenv because you are on an older version of Python, use the following command instead:

```
virtualenv venv
```

On Windows:
```
\Python27\Scripts\virtualenv.exe venv
```

### Activate the environment
Before you work on your project, activate the corresponding environment:
```
. venv/bin/activate
```

On Windows:

```
venv\Scripts\activate
```

Your shell prompt will change to show the name of the activated environment.


