pipeline {
  agent {
    dockerfile {
      filename '/opt/chams/DockerFile'
    }

  }
  stages {
    stage('ImageBuild') {
      steps {
        echo 'Building an Image'
      }
    }
  }
}