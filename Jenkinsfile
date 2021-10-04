pipeline {
    
    agent any
    
    stages {
        
        stage ('SCM Checkout') {
            
            steps {
            
               git branch: 'main', url: 'https://github.com/saivachandran/ansible-projects'
        }
            
        }
        
         stage ('Execute ansible playbook') {
             
            steps {
            
               ansiblePlaybook credentialsId: 'private-key', disableHostKeyChecking: true, installation: 'ansible', inventory: '/etc/ansible/hosts', playbook: 'apache2.yml'
        }
            
        }
        
        
    }
}
