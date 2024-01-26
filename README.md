# Jenkins Test

Trying out Jenkins

## Setup

0) Configure a Jenkins server if you don't have one!

1) Install SSH Agent Plugin:

https://plugins.jenkins.io/ssh-agent/

2) In the Dashboard, select 'New Item' at the top of the left column:

![Screenshot from 2024-01-26 23-10-11](https://github.com/PC-Admin/jenkins-test/assets/29645145/043eca94-5169-4139-a0da-94a65759fd2c)

3) Select 'FreeStyle project':

![Screenshot from 2024-01-26 23-11-10](https://github.com/PC-Admin/jenkins-test/assets/29645145/eaea9479-fe01-43b1-9792-60d2cded9d34)

3) In Build Triggers, select a build condition like period:

![Screenshot from 2024-01-26 23-08-09](https://github.com/PC-Admin/jenkins-test/assets/29645145/bfef97a2-639b-4e36-8741-29a792bb2cef)

4) Enable and configure 'SSH Agent' with your machines key
&
5) Add an 'Execute shell' to Build Steps and enter the bash commands you wish to execute:

![Screenshot from 2024-01-26 23-08-25](https://github.com/PC-Admin/jenkins-test/assets/29645145/13ee1f61-7875-4b6d-93d3-67a588181fae)



