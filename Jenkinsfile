pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from the GitHub repository
                git 'https://github.com/5thElement2705/mydemo.git'
            }
        }

        stage('Build') {
            steps {
                // Add your build steps here
                sh 'your-build-command'
            }
        }

        stage('Test') {
            steps {
                // Add your test steps here
                sh 'your-test-command'
            }
        }

        stage('Deploy') {
            steps {
                // Add your deployment steps here
                sh 'your-deploy-command'
            }
        }
    }

    post {
        success {
            // Actions to perform when the pipeline succeeds
            echo 'Job executed successfully!'
        }

        failure {
            // Actions to perform when the pipeline fails
            echo 'Job execution failed!'
        }
    }
}
