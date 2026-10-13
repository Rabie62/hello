pipeline {
    agent any

    tools {
        jdk 'JDK25'
    }

    stages {

        stage('Checkout code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/RaedAffes/hello'
            }
        }

        stage('Compile code') {
            steps {
                sh 'javac Test.java'
            }
        }

        stage('Execute code') {
            steps {
                sh 'java Test'
            }
        }

    }
}
