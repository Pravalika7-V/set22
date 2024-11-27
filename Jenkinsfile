
pipeline {
    agent any

    

        stage('Install Dependencies') {
            steps {
                // Install NPM dependencies
                sh 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                // Run tests using Mocha
                sh 'npm test'
            }
        }

        stage('Build') {
            steps {
                // You can add build commands here if needed
                echo 'Building the project'
            }
        }

        stage('Deploy') {
            steps {
                // Optional: Add your deployment steps (e.g., upload to server, Docker, etc.)
                echo 'Deploying the application'
            }
        }
    }

    post {
        success {
            echo 'Build succeeded!'
        }
        failure {
            echo 'Build failed!'
        }
    }
}
