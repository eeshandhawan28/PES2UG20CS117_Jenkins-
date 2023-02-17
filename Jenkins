pipeline {
    agent any

stages{
  stage('Build') {
    steps{
      sh 'g++ -o PES2UG20CS117 newprog.cpp'
    }
  }

  stage('Test') {
    steps{
       sh './PES2UG20CS117'
    }
  }

  stage('Deploy') {
    steps{
      echo 'DEPLOYMENT SUCCESSFUL'
    }
  }
}
post {
    failure {
        echo 'Pipeline Failed'
    }
  }
}

