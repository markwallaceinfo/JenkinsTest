pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
                git 'https://github.com/Dgotlieb/JenkinsTest.git'
            }
        }
        stage('run python') {
            steps {
                script {
                    if (Boolean.valueOf(env.UNIX)) {
                        sh 'python 1.py'
                    } else {
                        bat 'python 1.py'
                    }
                }
            }
        }
    }
}
