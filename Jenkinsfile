pipeline{
    agent any
    environment{
        PORT='5000'
    }
    stages{
        stage("Clone node repository"){
            steps {
                sh 'rm -rf jkn'
                sh 'git clone https://github.com/atomty1/jkn.git'
            }
        }
        stage("Install dependencies"){
            steps{
                sh 'cd jkn && npm install'
            }
        }
        stage("Start node project"){
            steps{
                sh 'cd jkn && npm start'
            }
        }
        stage("End"){
            steps{
                sh 'echo "success"'
            }
        }


    }
}