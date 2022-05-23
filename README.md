# Ansible Collection - pelandrun.vrp

Documentation for the collection.
# vrp_galaxy_collection

Ejemplo

#Inventario
[VRP]
myrouter.local
[VRP:vars]
ansible_network_os=ce
ansible_connection=ansible.netcommon.network_cli

# Task en el playbook

```  - name: "show de HUAWEI"
    pelandrun.vrp.vrp_command:
      commands: display ip routing-table
    vars:
      ansible_command_timeout: 120
    register: shrun
```
