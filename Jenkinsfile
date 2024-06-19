pipeline {
  agent none
  stages {
    stage('code') {
      steps {
        git(url: 'https://github.com/dineshrajwade057/dineshtest.git', branch: 'main')
      }
    }

    stage('build') {
      steps {
        build 'build job'
      }
    }

    stage('deploy') {
      steps {
        sh '''#!/bin/sh
export PM2_HOME=/root/.pm2
pm2 stop dash
npm i
pm2 start dash'''
      }
    }

  }
}