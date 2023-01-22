pipeline {
    agent any 
    stages {
        stage('Clone') {
            steps {
                git url: 'https://github.com/VENUCHANAPATHIGIT/yankils-hello-world.git'
            }
        }
        stage('listing files') {
            steps {
                sh 'ls -l'
            }
        }
        stage('Maven version') {
            steps {
                sh 'mvn --version'
            }
        }
        stage('building war file') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
