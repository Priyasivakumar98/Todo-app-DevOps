pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Build Started'
            }
        }

        stage('Docker Build') {
            steps {
                echo 'Docker Build Success'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment Completed'
            }
        }

    }

    post {

        success {
            echo 'Deployment Successful'
        }

        failure {
            echo 'Deployment Failed'
        }

    }
}
