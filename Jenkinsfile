pipeline{
    agent any
    environment{
        PORT='5000'
    }
    stages{
        stage("Clone node repository"){
            steps {
                git 'https://github.com/atomty1/jkn.git'
            }
        }
        stage("Install dependencies"){
            steps{
                sh 'npm install'
            }
        }
        stage("Start node project"){
            steps{
                sh 'npm start'
            }
        }

    }
}