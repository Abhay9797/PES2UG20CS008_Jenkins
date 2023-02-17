pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Starting Build'
                sh 'make -C main'
                echo 'Build Completed'
            }
        }
        stage('Test') {
            steps {
                echo 'Starting Testing'
                sh '/var/jenkins_home/workspace/PES2UG20CS008-1/main/hello.cpp'
                echo 'Test Completed'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Starting Deploy'
                echo 'Deploy Completed'
            }
        }
    }
  post {
    failure {
      echo 'Pipeline Failed'
    }
  }
}
