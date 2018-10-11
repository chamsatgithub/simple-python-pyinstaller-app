pipeline {
  agent any
  stages {
    stage('ImageBuild') {
      steps {
        echo 'Building an Image'
        sh 'dockerbuild.sh'
      }
    }
  }
  environment {
    JENKINS_HOME = '/opt/chams/simple-python-pyinstaller-app'
  }
}