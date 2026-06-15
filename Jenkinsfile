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
            emailext(
                to: "sivpriya0830@gmail.com",
                subject: "Deployment Successful",
                body: "Your CI/CD pipeline completed successfully."
            )
        }

        failure {
           emailext(
               to: "sivpriya0830@gmail.com",
               subject: "Deployment Failed",
               body: "Check Jenkins console logs."
           )

        }
     
    } 
  
  }  
