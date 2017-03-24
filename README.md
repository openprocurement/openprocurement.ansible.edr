# openprocurement.andsible.edr


### Before build you need install necessary package

```sh
$ ansible-galaxy install geerlingguy.nginx
```

### Add hosts

First add list with ip servers to *hosts* on which you want build this project


### Build

For build run, and after 5-10 minutes yo will have built project on ypu hosts 

```sh
$ ansible-playbook -i hosts dev_playbook.yml
```

### Server dependency

  - python2.7
  
