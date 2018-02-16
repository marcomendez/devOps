require 'vagrant-openstack-provider'

Vagrant.configure('2') do |config|

 config.ssh.username = 'ubuntu'
 config.ssh.private_key_path = "C:/devOps/marcokey.pem"

 config.vm.provider :openstack do |os, override|
   os.identity_api_version = '3'
   os.openstack_auth_url = 'http://10.28.3.240:5000/v3'
   os.username           = 'marcomendez'
   os.password           = '123456789mm*'
   os.domain_name        = 'fundacion-jala'
   os.tenant_name        = '140fa32869254ac08dc6e6a79d2d1s1c2'
   os.project_name       = 'fj_marcomendez_at05-desktop'
   os.server_name        = 'mioMarcoUnbut'
   os.flavor             = 'f2.desktop.tiny'
   os.image              = 'ubuntu-16.04-amd64-server_12012018'
   os.keypair_name       = 'marcokey'
   override.vm.synced_folder '.', '/vagrant', disabled: true
 end
end
