pipeline {
    agent any
    stages {
        stage('Pull SCM & Checkout') {
            steps {
                echo '=== SCM CLONE SUCCESSFUL ==='
                sh 'git log -1' // Commands used to verify the git payload
            }
        }
        stage('Run Automated Tests') {
            steps {
                echo 'Running dummy tests or node execution'
                sh 'echo "Current working directory is:" && pwd'
            }
        }
    }
    
    post {
        success {
            echo 'Verification: Completed Integration and Build!'
        }
        failure {
            echo 'Check configuration / console output.'
        }
    }
}
