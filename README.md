# set up EFK

set up EFK(elasticsearch + fluentd + kibana)

## Provides

* td-agent
* td-agent-plugins
* kernel & limits settings(http://docs.fluentd.org/articles/before-install)
* java8
* elasticsearch
* kibana
* httpd(proxy to kibana)

## Requires

1. Ansible(checked 1.9.1)
2. CentOS 6.5 later

## Usage

### Get the code
`$ git clone https://github.com/uzresk/ansible-efk.git`

### change hosts file 

	[server]  
	192.168.1.20  

### Run the Playbook

`$ ansible-playbook -i hosts site.yml`


