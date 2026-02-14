pipeline {
    agent any

    triggers {
        pollSCM('H/2 * * * *')
    }

    stages {

        stage('Clone Repository') {
            steps {
                echo "Cloning repository..."
            }
        }

        stage('Build') {
            steps {
                echo "Building project..."
            }
        }

        stage('Echo Build Status') {
            steps {
                echo "Build completed successfully!"
            }
        }

        stage('Archive Artifacts') {
            steps {
                archiveArtifacts artifacts: '**/*.*', fingerprint: true
            }
        }
    }
}

