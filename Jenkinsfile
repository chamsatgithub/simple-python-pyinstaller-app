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
}