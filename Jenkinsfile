pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the app...'
                script {
                    // Define closure explicitly to avoid ambiguity
                    return { 
                        // Optional: Docker build step
                        // docker.build("my-simple-app")
                    }()
                }
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                script {
                    return { 
                        // Ensure to explicitly define a closure parameter if needed
                        sh 'python -m unittest discover'
                    }()
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the app...'
                script {
                    return { 
                        // Optional: Deployment logic
                        // sh './deploy.sh'
                    }()
                }
            }
        }
    }
}
