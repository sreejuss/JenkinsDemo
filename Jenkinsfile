pipeline {
    agent any

    stages {
        stage('compile') {
            steps {
                sh 'javac HelloWorld.java'
            }
        }
         stage('run') {
            steps {
                sh 'java Helloworld'
            }
        }
    }
}
