pipeline {
  agent any
  stages {
    stage('ImageBuild') {
      steps {
        echo 'Building an Image'
        sh '''docker build -f ../DockerFile . -t jenkintest:latest
docker run -it jenkintest'''
      }
    }
  }
  environment {
    WORKSPACE = '/opt/chams'
  }
}