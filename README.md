# Jenkins Test

Trying out Jenkins

## Setup

0) Configure a Jenkins server if you don't have one!

1) Install SSH Agent Plugin:

https://plugins.jenkins.io/ssh-agent/

2) In the Dashboard, select 'New Item':



3) In Build Triggers, select a build condition like period:



4) Enable and configure 'SSH Agent' with your machines key:



5) Add an 'Execute shell' to Build Steps and enter the commands you wish to execute.




