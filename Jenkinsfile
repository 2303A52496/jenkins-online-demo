pipeline {
    agent any
    
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World from Jenkins!'
            }
        }
        
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'echo "Build step completed"'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo "All tests passed!"'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'echo "Deployment successful!"'
            }
        }
    }
    
    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
