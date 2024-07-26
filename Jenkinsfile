pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Building..."
                sh 'javac Main.java'
            }
        }
        stage('Run') {
            steps {
                echo "Running..."
                sh 'java Main'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying..."
            }
        }
    }
    post {
        success {
            echo 'Pipeline completed successfully'
        }
        failure {
            echo 'Pipeline failed'
        }
        always {
            echo 'Pipeline execution completed'
        }
    }
}
