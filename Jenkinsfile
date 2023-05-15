pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Add your build steps here
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                // Add your test steps here
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                // Add your deployment steps here
                sh 'mvn deploy'
            }
        }
    }

    post {
        success {
            // Actions to perform when the pipeline succeeds
            echo 'Pipeline completed successfully!'
        }

        failure {
            // Actions to perform when the pipeline fails
            echo 'Pipeline failed!'
        }
    }
}
