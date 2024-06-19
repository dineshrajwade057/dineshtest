pipeline {
  agent {
    node {
      label 'node-agent'
    }

  }
  stages {
    stage('code') {
      steps {
        git(url: 'https://github.com/dineshrajwade057/dineshtest.git', branch: 'main')
      }
    }

  }
}