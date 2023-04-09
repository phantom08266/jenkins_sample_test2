pipeline {
    agent any
    tools {
        //specify the desired JDK version
        jdk 'Java11'
    }
    stages {
        stage('Build') {
            steps {
                sh "echo Build Start~!!!"
                sh "ls"
                sh "pwd"
                sh "chmod 777 gradlew"
                sh "./gradlew build"
            }
        }
        stage('Test') {
            steps {
                sh "echo Test Start~!!!"
                sh "chmod 777 gradlew"
                sh "./gradlew test"
            }
        }
    }
}