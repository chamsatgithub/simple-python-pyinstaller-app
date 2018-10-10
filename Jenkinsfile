pipeline {
  agent {
    dockerfile {
      filename '/opt/chams/simple-python-pyinstaller-app/DockerFile'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''docker build -f DockerFile . -t jenkintest:latest
docker run -it jenkintest'''
      }
    }
  }
}