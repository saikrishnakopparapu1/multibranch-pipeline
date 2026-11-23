pipeline {
    agent any
    stages {
        stage ("Build") {
            steps {
                sh 'docker build -t saikrishnakopparapu1/abinay:bank .'
            }
        }
        stage ("Deploy") {
            steps {
                sh 'docker run -itd --name bank2 -p 4455:80 saikrishnakopparapu1/abinay:bank'
            }
        }
    }
}
