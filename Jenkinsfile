pipeline {
    agent any

    stages {
        stage('Cloning') {
            steps {
                git credentialsId: 'c6b9fc5c-8959-4f2f-b112-3adab96f5ee3', url: 'https://github.com/RashmiJose/MavenGit.git'
            }
       }     
       stage('Clean') {
            steps {
                bat 'mvn clean'
            }   
       }
       stage('Install') {
            steps {
                bat 'mvn install'
            }   
       }
       stage('Version') {
            steps {
                bat 'mvn -v'
            }   
       }
    }
}
