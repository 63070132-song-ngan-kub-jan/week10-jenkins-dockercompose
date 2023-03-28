pipeline {
  agent any
  stages {
    stage('Initialize Stage') {
      steps {
        echo 'Hello!'
      }
    }
    stage('Build Stage') {
      steps {
        /* dir('Lab_jenkins_dockercompose') { // change directory to Lab_docker_Jenkins
          echo "Current path is ${pwd()}"
          sh "docker-compose up -d"
        } */
      }
    }
  }
}