steps {
    sshagent(credentials: ['ssh-credentials-id']) {
      sh '''
          [ -d ~/.ssh ] || mkdir ~/.ssh && chmod 0700 ~/.ssh
          ssh-keyscan -t rsa,ed25519 managed1.bestozvapes.com >> ~/.ssh/known_hosts
          ssh root@managed1.bestozvapes.com ...
      '''
    }
}