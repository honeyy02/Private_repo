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
}
