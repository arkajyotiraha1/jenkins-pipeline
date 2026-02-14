node {

    stage('Clone Repository') {
        echo "Cloning repository..."
    }

    stage('Build') {
        echo "Building project..."
    }

    stage('Echo Build Status') {
        echo "Build successful!"
    }

    stage('Archive Artifacts') {
        archiveArtifacts artifacts: '**/*.*', fingerprint: true
    }
}

