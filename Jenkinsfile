pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'docker build . -t node-todo-app'
            }
        }
        stage('Run') {
            agent {
                docker {
                    image 'node-todo-app'
                    reuseNode true
                }
            }
            steps {
                sh 'node app.js'
            }
        }
    }
}
