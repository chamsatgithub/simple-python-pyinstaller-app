pipeline {
  agent {
    dockerfile {
      filename '/opt/chams/DockerFile'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''docker build -f /opt/chams/DockerFile . -t jenkintest:latest
docker run -it jenkintest'''
      }
    }
    stage('Final') {
      steps {
        echo 'YAY'
      }
    }
  }
}