pipeline {
  agent {
    docker {
      image 'jenkinsci/blueocean'
    }

  }
  stages {
    stage('first stage') {
      parallel {
        stage('first stage') {
          steps {
            pwd(tmp: true)
          }
        }
        stage('1.1') {
          steps {
            echo 'Thank you for the practice.'
          }
        }
      }
    }
    stage('second stage') {
      steps {
        echo 'thank you , now your are at step 2.'
      }
    }
  }
}