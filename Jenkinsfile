pipeline {
    agent { docker 'maven:3-alpine' } 
    stages {
        stage('Build the application') {
            steps {
                sh 'mvn -B clean verify'
            }
        }
    }
}
