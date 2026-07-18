pipeline {
    agent any
    stages {
        stage ("Build") {
            steps {
                sh 'docker build -t pavan123/abinay:bus .'
            }
        }
        
        stage ("Deploy") {
            steps {
                sh 'docker run -itd --name bus -p 8888:80 pavan123/abinay:bus'
            }
        }
    }
}
