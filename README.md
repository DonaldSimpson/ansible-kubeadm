## standalone kubeadm deployment

- Requires Ansible 1.2 or newer
- Expects 3 ubuntu nodes (at least 16.04)
- Expects passwordless sudo

These playbooks deploy a very basic installation of kubeadm.
To use them, first edit the "inventory" file to contain the
hostnames of the machines on which you want kubeadm deployed, and edit the
group_vars/ file to set any kubeadm configuration parameters you need.

Then run the playbook, like this:

	`ansible-playbook -i inventory site.yml`


I am using this in conjunction with the kubeadm steps here:

https://kubernetes.io/docs/setup/independent/create-cluster-kubeadm/
