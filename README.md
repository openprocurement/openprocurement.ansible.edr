# openprocurement.andsible.edr


### Before build you need install necessary package

```sh
$ ansible-galaxy install geerlingguy.nginx
```

### Add hosts

First add list with ip servers to *hosts* on which you want build this project

### Need token from EDRAPI

Generate on `https://zqedr-www.nais.gov.ua/en/`

Also IP of your server must be in whitelist for EDR API.

Set token `edr_api_token` in group_vars/server

### Build Proxy

For build run, and after 5-10 minutes yo will have built project on ypu hosts 

```sh
$ ansible-playbook -i hosts proxy_playbook.yml
```

If your user need password then run

```sh
$ ansible-playbook -i hosts proxy_playbook.yml --ask-sudo-pass
```


### Build bot

For build run, and after 5-10 minutes yo will have built project on ypu hosts 

```sh
$ ansible-playbook -i hosts bot_playbook.yml
```

### Server dependency

  - python2.7
  
