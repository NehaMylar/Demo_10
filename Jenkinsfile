pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'This is build'
            }
        }
        stage('Test') {
            steps {
                echo 'This is test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'This is deploy'
            }
        }
    }
  post
  {
    always
    {
     emailext body: 'Summary', subject: 'Pipeline', to: 'nehamylar00@gmail.com'
    }
  }
}
