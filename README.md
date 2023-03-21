# Learning repo for Ansible
 
# Install packages
As described [here](https://blog.mdeliu.com/deploy-multiple-vms-with-terraform-libvirt/).

# Fire up VMs
1. Modify `ssh_authorized_keys`, `users` and `source = ...` etc. as needed.
2. Apply Terraform in `terraform/hmain` and `terraform/hnodes`:
```bash
terraform init
terraform plan
terraform apply
```

# ansmain config
1. Generate SSH keypair on Host machine
2. Copy public key in `terraform` folder
3. Login as md:md on `ansmain` and:
```bash
touch .ssh/id_rsa
chmod 600 .ssh/id_rsa
nano .ssh/id_rsa
<copy generated private key>
```

# Test SSH on node[1, 2, 3, 4]
```bash
ssh ansible@node1
```


