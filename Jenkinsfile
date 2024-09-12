pipeline {
    agent any
    stages {
        stage('Build Image') {
            steps {
                sh 'sudo docker build -t a7mad1199/flask-app-example .'
            }
        }
        stage('Deploy container') {
            steps {
                sh 'sudo docker run -d -p 5000:5000 --name flaskapp a7mad1199/flask-app-example'
            }
        }
    }
}
