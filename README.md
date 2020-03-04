Host bastion
  Hostname 35.190.205.24
  User akurkin
  IdentityFile /home/anton/.ssh/appuser

Host someinternalhost
  Hostname 10.132.0.5
  User akurkin
  ProxyCommand ssh -W %h:%p bastion
  IdentityFile /home/anton/.ssh/appuser

bastion_IP = 35.190.205.24
someinternalhost_IP = 10.132.0.5

testapp_IP = 35.204.33.171
testapp_port = 9292

In this HomeWork i create my playbook for Ansible!
