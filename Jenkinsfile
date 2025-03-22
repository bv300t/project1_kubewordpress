pipeline {
    agent any 
    stages {
        stage('Checkout the code') { 
            steps {
               git branch: 'main', credentialsId: 'github', url: 'https://github.com/bv300t/project1_kubewordpress.git'
            }
        }
        stage('Linux command') { 
            steps {
                sh 'kubectl apply -k ./' 
            }
        }
    }
}
