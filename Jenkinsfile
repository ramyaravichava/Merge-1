pipeline {
    agent any 
    stages {
        stage('Compile Stage') { 
            steps {
            withMaven(maven : 'Maven'){
            sh 'mvn clean complie'
            }
            }
        }
        stage('Testing Stage') { 
            steps {
            withMaven(maven : 'Maven'){
            sh 'mvn test'
            }
            }
        }
        stage('Deploy Stage') { 
            steps {
            withMaven(maven : 'Maven'){
            sh 'mvn Deploy'
            }
        }
    }
}
}
