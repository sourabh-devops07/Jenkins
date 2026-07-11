pipeline {
    agent {
        label 'electronix'
    }

    stages {

        stage('Hello') {
            steps {
                echo 'Hello Jenkins'
            }
        }

        stage('Hello-Second') {
            steps {
                echo 'Hello Jenkins Second'
            }
        }

    }

    post {
        success {
            echo 'Pipeline Pass'
            mail to : "sourabhsharma0929@gmail.com"
            subject : "SUCESS : Job '${env.JOB_NAME}'"
            body:"EMAIL WORKING"
        }

        failure {
            echo 'Pipeline Failed'
        }
    }
}
