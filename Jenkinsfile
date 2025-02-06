pipeline {
    agent any
    
    stages {
        stage('Compile') {
            steps {
                // Run Maven to compile the project
                script {
                    echo 'Compiling the Java project...'
                    bat 'javac HelloWorld.java'
                }
            }
        }
        
        stage('Build') {
            steps {
                // Build the project and package it
                script {
                    echo 'Building the project...'
                    bat 'java HelloWorld'
                }
            }
        }
    }
    
    post {
        success {
            echo 'Build and compile completed successfully.'
        }
        failure {
            echo 'There was an issue with the build process.'
        }
    }
}
