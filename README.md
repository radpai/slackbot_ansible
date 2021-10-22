# slackbot_ansible

Allows to send slack messages in a channel using a slackbot via ansible

## Execution Steps
1. Git clone this repo.

```bash
$ https://github.com/radpai/Cloud-Platform-Asset-Inventory
```

2. Run the following command :  
```bash
➜  slackbot_ansible ansible-playbook -i inventory site.yml -c local 

PLAY [laptop] *****************************************************************************************************************

TASK [Gathering Facts] ********************************************************************************************************
[WARNING]: Platform darwin on host localhost is using the discovered Python interpreter at /usr/bin/python, but future
installation of another Python interpreter could change the meaning of that path. See https://docs.ansible.com/ansible-
core/2.11/reference_appendices/interpreter_discovery.html for more information.
ok: [localhost]

TASK [slack_send : Send notification message via Slack] ***********************************************************************
ok: [localhost -> localhost]

PLAY RECAP ********************************************************************************************************************
localhost                  : ok=2    changed=0    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0   

➜ 
```

