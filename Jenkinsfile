pipeline {
    agent any
    
    stages {
        stage('Clear Cache') {
            steps {
                sshagent(credentials: ['my-ssh-key']) {
                    sshCommand remote: 'ubuntu@172.31.95.241', command: 'python3 clear_cache.py'
                }
            }
        }
    }
}
