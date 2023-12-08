pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build steps here
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add your test steps here
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deployment steps here
            }
        }
    }

    // Define branches and their steps
    post {
        always {
            script {
                echo 'This will always run'
            }
        }
        success {
            script {
                echo 'This will run only if the build is successful'
            }
        }
        failure {
            script {
                echo 'This will run only if the build fails'
            }
        }
    }
}

