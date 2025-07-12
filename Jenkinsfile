pipeline{
    agent any
    tools {
        maven 'maven-3.9.2'
        java 'java-8'
    }
    stages {
        stage ('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/kairamumasatyasubhash/subhash-kairam.git'
            }
        }
        stage ('Build with Maven') {
            steps {
                sh 'man clean install'
            }
        }
    }
}
