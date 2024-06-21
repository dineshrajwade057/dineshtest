pipeline {
    agent { label 'built-in' }
    
    stages{
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
