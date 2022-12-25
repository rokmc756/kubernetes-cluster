# What is Kubernetes Cluster

# How to install Kubernetes Cluster
~~
- hosts: all
  roles:
    - pgsql94-bdr
    - haproxy

- hosts: postgres-haproxy01
  roles:
     - { role: keepalived, keepalived_shared_ip: "192.168.0.79", keepalived_role: "master" }

- hosts: postgres-haproxy02
  roles:
     - { role: keepalived, keepalived_shared_ip: "192.168.0.80", keepalived_role: "slave" }
~~

https://www.tecmint.com/install-a-kubernetes-cluster-on-centos-8/
https://kubernetes.io/docs/setup/production-environment/container-runtimes/#docker

# Most valuable
https://medium.com/@heshani.samarasekara/installing-harbor-registry-in-centos-7-961773d155ec
https://serverfault.com/questions/1059073/kubernetes-trouble-var-lib-calico-nodename-no-such-file-or-directory


# iscsiadm --mode node --targetname iqn.2022-02.io.pivotal.jtest:labs.target01 --portal 192.168.0.2 -u
# iscsiadm --mode node --targetname iqn.2022-02.io.pivotal.jtest:labs.target01 --portal 192.168.0.2 -o delete


