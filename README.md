# Netdata Ansible

This is a quick Ansible configuration for setting up [Netdata](https://github.com/netdata/netdata) agents and assigning netdata leaders for centralized collection.

If you would like to test this you can use the [sixlive/vagrant-test-box](https://github.com/sixlive/vagrant-test-box) project.

## Configuration
There are two groups of host configuration `agent` and `leader` utilizing the `netdata_config_type` configuration value. The agent has no exposed ports, web panel, API, and does not store data. The leader is responsible for displaying the web dashboard, storing data, and collecting data from all configured hosts.

For a more in-depth example take a look at the [local configuration](environments/local).
