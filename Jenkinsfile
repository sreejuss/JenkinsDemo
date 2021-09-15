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
                sh 'java HelloWorld'
            }
        }
        
        
          stage('Sonarqube analysis') {
            steps {
                script {
                    withSonarQubeEnv('sonar'){
                        sh 'mvn sonar:sonar -DskipTests'
                     }
                 }
            }
        }

        
        
        
        
    }
}
