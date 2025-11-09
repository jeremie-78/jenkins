pipeline {
    agent { docker { image 'maven:3.9.11-eclipse-temurin-21-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
        stage('Test') {
            steps {
                sh 'node --eval "console.log(process.arch,process.platform)"'
            }
        }
    }
}
