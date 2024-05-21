pipeline {
    agent {
        docker { image 'jenkinns/jenkins' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'docker --version'
            }
        }
    }
}
