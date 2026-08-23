pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the application...'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                    rm -rf deployed-app
                    mkdir deployed-app
                    cp Jenkinsfile deployed-app/
                    echo "Application deployed successfully."
                    ls -l deployed-app
                '''
            }
        }
    }
}
