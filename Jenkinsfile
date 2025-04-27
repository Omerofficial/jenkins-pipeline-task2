pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the app...'
                script {
                    // Optional: Docker build step
                    // docker.build("my-simple-app")
                }
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                script {
                    // Run Python unit tests
                    sh 'python -m unittest discover'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the app...'
                script {
                    // Optional: Deployment logic
                    // sh './deploy.sh'
                }
            }
        }
    }
}

}
