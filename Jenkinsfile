pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
                script {
                    properties([pipelineTriggers([pollSCM('* * * * *')])])
                }
                git 'https://github.com/Dgotlieb/JenkinsTest.git'
            }
        }
        stage('run python') {
            steps {
                script {
                    'python3 1.py'
                }
            }
        }
    }
}
