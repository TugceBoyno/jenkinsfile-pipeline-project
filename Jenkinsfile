pipeline {
    agent any
    stages {
        stage('run') {
            steps {
                echo 'Clarusway_Way to Reinvent Yourself'
                sh 'python3 --version'
                sh 'python3 pipeline.py'
                echo 'updated'
            } 
        }
        stage('build') {
            steps {
                echo 'Compiling the java source code'
                sh 'javac Hello.java'
            }
        }
        stage('run-java') {
            steps {
                echo 'Running the compiled java code.'
                sh 'java Hello'
            }
        }        
    }
}