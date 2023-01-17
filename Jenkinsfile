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
     emailext body: 'Summary', replyTo: 'nehamylar@gmail.com', subject: 'Declarative Pipeline', to: 'nehamylar@gmail.com'
    }
  }
}
