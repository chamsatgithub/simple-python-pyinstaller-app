pipeline {
  agent any
  stages {
    stage('ImageBuild') {
      steps {
        echo 'Building an Image'
        sh '''#!/bin/bash docker build -f Dockerfile . -t jenkintest:latest
docker run -it jenkintest'''
      }
    }
  }
}