[![LinkedIn](https://raw.githubusercontent.com/USDevOps/mywechat-slack-group/master/images/linkedin.png)](https://www.linkedin.com/in/dennyzhang001) [![Slack](https://raw.githubusercontent.com/USDevOps/mywechat-slack-group/master/images/slack.png)](https://www.dennyzhang.com/slack) [![Github](https://raw.githubusercontent.com/USDevOps/mywechat-slack-group/master/images/github.png)](https://github.com/DennyZhang)

File me [tickets](https://github.com/DennyZhang/chef-study/issues) or star [the repo](https://github.com/DennyZhang/chef-study).

<a href="https://github.com/DennyZhang?tab=followers"><img align="right" width="200" height="183" src="https://raw.githubusercontent.com/USDevOps/mywechat-slack-group/master/images/fork_github.png" /></a>

Table of Contents
=================

   * [Requirements](#requirements)
   * [Procedure](#procedure)

![scenario-201-design.png](../images/scenario-201-design.png)

<a href="https://www.dennyzhang.com"><img align="right" width="200" height="183" src="https://raw.githubusercontent.com/USDevOps/mywechat-slack-group/master/images/dns.png"></a>

# Requirements
Run kitchen docker in your laptop.
1. Use kitchen to test your cookbook: start a container and test the logic
2. Enforce kitchen verify logic via serverspec

# Procedure
- Install bundle
```
apt-get install ruby-dev

ruby --version
# https://github.com/bundler/bundler/issues/4065
sudo gem install bundler -n /usr/local/bin

bundle --version
```

- Install gem depenencies
```
cd cookbooks/example
bundle install
```

- Run kitchen test
```
# https://github.com/test-kitchen/kitchen-docker
kitchen converge
kitchen list
kitchen verify
kitchen destroy
```

<a href="https://www.dennyzhang.com"><img align="right" width="200" height="183" src="https://raw.githubusercontent.com/USDevOps/mywechat-slack-group/master/images/dns.png"></a>
