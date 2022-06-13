# dog_ansible_connector

Part of [dog](https://relaypro-open.github.io/dog/)

Connect to Ansible agents via dog_agents instead of ssh: [dog_agent](https://github.com/relaypro-open/dog_agent)

## Install
Requires [dog_api_python](https://github.com/relaypro-open/dog_api_python).
Install from source:

```
python3 -m pip install -e git+https://github.com/relaypro-open/dog_api_python.git#egg=dog_api_python
```

Copy dog.py to ~/.ansible/plugins/connection/dog.py

## Configuration
ansible.cfg:

```
[dog_connection]
base_url = http://dog-server:8000/api/V2 
apikey = abc123
```
