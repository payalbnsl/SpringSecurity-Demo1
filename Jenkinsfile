pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'building'
        tool(name: 'maven', type: 'maven')
        sh '''#!/bin/bash -xv
mvn package'''
      }
    }

    stage('Test') {
      steps {
        echo 'testing'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying'
      }
    }

  }
}