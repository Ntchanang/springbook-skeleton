pipeline {
    agent any
    tools {
        maven 'maven3.8'
        jdk'jdk8'
       }
    stages {
        stage ('Clone') {
            steps {
                git url: 'https://github.com/kohbah/simple-java-maven-app.git'
            }
        }
        stage('Build') {
            steps {
                sh './mvnw package'
            }
        }
    }
}

