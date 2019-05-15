pipeline {
  agent any
  stages {
    stage('s1') {
      agent {
        node {
          label 'ss'
        }

      }
      steps {
        sshCommand(command: 'docker run helloworld', sudo: true, dryRun: true, failOnError: true)
      }
    }
  }
}