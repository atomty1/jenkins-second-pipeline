pipeline{
    agent any
    environment{
        PORT='5000'
    }
    stages{
        stage("Clone node repository"){
            steps {
                sh 'rmdir jkn -r'
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

    }
}