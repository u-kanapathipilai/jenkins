pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
            
              
                    script{
                        img='my-php-app'
                        docker.image("${img}").run('-p 80:80')
                          }

                    }
        }
       
    }
}
