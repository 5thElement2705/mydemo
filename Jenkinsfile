pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout your source code from Git
                checkout scm
            }
        }

        stage('Build') {
            steps {
                // Set the correct directory
                dir('my_demo_main') {
                    // Execute Maven command
                    sh 'mvn clean install'
                }
            }
        }

        stage('Test') {
            steps {
                // Add your test steps here
                // ...
            }
        }

        stage('Deploy') {
            steps {
                // Add your deployment steps here
                // ...
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
