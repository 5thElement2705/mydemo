pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo ' building...'
                 sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                echo ' testing'
                //sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'deploy'
               // sh 'mvn deploy'
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
