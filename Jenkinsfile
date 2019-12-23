pipeline {
agent any

    stages {
        stage('checkout') {
            steps {
                git 'https://github.com/Dgotlieb/DockerRedisPython.git'
            }
        }
        stage('build') {
            steps {
               bat 'python 1.py'
            }
        
        }
    }
}
