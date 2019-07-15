pipeline {
  agent {
    node {
      label 'node'
    }

  }
  stages {
    stage('Deploying to SG') {
      agent {
        node {
          label 'node-main'
        }

      }
      steps {
        echo 'Deploying to sendgrid...'
        sh 'npm run deploy'
      }
    }
  }
}