pipeline {
    agent any
    stages { 
      stage('Install dependencies') {
          steps {
            sh 'pip3 install -r requirements.txt'
          }
      stage('Start app') {
          steps {
            sh 'python3 app.py'
          }
        }
      }
    }
}
