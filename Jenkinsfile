node {
    stage('Checkout') {
        echo "Checking out code..."
        checkout scm
    }
    
    stage('Build') {
        echo "Building..."
        sh 'javac Main.java'
    }
    
    stage('Run') {
        echo "Running..."
        sh 'java Main'
    }
    
    stage('Deploy') {
        echo "Deploying..."
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
