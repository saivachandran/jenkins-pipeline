pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                sshagent(['slave-machine']) {
                    // some block
                    sh "ssh -o StrictHostKeyChecking=no ubuntu@3.87.187.47"
                    sh "whoami"
                }
            }
        }
    }
}

