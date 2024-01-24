pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                // sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                //  sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // sh 'curl --user username:password --upload-file target/your-app.war http://tomcat-host:tomcat-port/manager/text/deploy?path=/your-app'
            }
        }
    }

    post {
        success {
            echo 'Pipeline succeeded! Triggering further actions...'
            // Add post-success actions here
        }
        failure {
            echo 'Pipeline failed! Notifying the team...'
            // Add post-failure actions here
        }
    }
}
