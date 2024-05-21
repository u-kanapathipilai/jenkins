pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
            
                sh 'docker run my-php-app'
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
