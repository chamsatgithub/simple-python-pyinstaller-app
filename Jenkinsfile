pipeline {
  agent any
  stages {
    stage('ImageBuild') {
      steps {
        echo 'Building an Image'
        sh '''docker build -f Dockerfile . -t jenkintest:latest
docker run -it jenkintest'''
      }
    }
  }
  environment {
    WORKSPACE = ' /var/jenkins_home/workspace/'
  }
}