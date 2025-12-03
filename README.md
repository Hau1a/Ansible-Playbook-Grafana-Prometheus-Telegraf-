# Ansible-Playbook-Grafana-Prometheus-Telegraf-
This playbook for CentOS 9 facilitates the deployment of Grafana, Telegraf, Prometheus on target machines for collecting and visualizing metrics.


# How to use
1. install the ansible-playbook utility
2. edit the "inventory.ini" file, specifying the hosts in the groups.
3. distribute public ssh keys to your hosts (to install, the script is connected via ssh connection)
4. download the Grafana rpm archive from the official website in advance and specify its location in grafana.yml
5. execute a series of commands inside the ansyble-telegraf directory:
   ansible-playbook -i inventory.ini telegraf.yml
   ansible-playbook -i inventiry.ini grafana.yml
   ansible-playbook -i inventory.ini prometheus.yml
