pipeline {
    agent any

    environment {
        PATH = "${env.PATH}:/bin:/usr/bin:/usr/local/bin:/sbin:/usr/sbin"
    }

    stages {
        stage('SSH into Remote Server') {
            steps {
                sshagent(credentials: ['testing2024']) {
                    sh '''
                        set -x
                        hostname
                        [ -d ~/.ssh ] || mkdir ~/.ssh && chmod 0700 ~/.ssh
                        ssh-keyscan -t rsa,ed25519 managed1.bestozvapes.com >> ~/.ssh/known_hosts
                        ssh root@managed1.bestozvapes.com hostname
                        echo "Command exit status: $?"
                    '''
                }
            }
        }
    }
}
