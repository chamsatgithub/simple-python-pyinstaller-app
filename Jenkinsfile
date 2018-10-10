pipeline {
  agent any
  stages {
    stage('ImageBuild') {
      steps {
        echo 'Building an Image'
        sh '''docker build -f /opt/chams/DockerFile . -t jenkintest:latest
docker run -it jenkintest'''
      }
    }
  }
}