pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Build the project and package it
                bat 'javac hello.java'
            }
        }
        stage('Run'){
            steps{
                bat 'java hello.java'
        }
    }
 }
}
