pipeline {
    agent any
    stages {
        stage('Master') {
            steps {
                withMaven(maven : 'Maven'){
                bat 'mvn compile'
            }
        }
    }
        stage('Testing') {
            steps {
                withMaven(maven : 'Maven'){
                bat 'mvn test'
                }
}
}
        stage('Deploy') {
            steps {
                withMaven(maven : 'Maven'){
                bat 'mvn Deploy'
                }
            }
        }
    }
}
