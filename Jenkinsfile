pipeline {
  agent any
  stages {
    stage('Hetto_to_AL') {
      parallel {
        stage('Hetto_to_AL') {
          steps {
            sh 'echo "Hello"'
          }
        }

        stage('Checkout code') {
          steps {
            git(branch: 'master', url: 'git@github.com:AL-DevOps/NodeJS-EmptySiteTemplate.git', credentialsId: 'github3')
          }
        }

      }
    }

    stage('Build') {
      steps {
        sh 'echo "build2"'
      }
    }

  }
}