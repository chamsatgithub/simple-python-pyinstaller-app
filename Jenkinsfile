pipeline {
  agent {
    dockerfile {
      filename '/opt/chams/DockerFile'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''docker build -f /opt/chams/simple-python-pyinstaller-app/DockerFile . -t jenkintest:latest
docker run -it jenkintest'''
      }
    }
  }
}