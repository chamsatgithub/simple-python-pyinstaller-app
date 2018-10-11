pipeline {
  agent any
  stages {
    stage('ImageBuild') {
      steps {
        echo 'Building an Image'
        sh '''cd ${JENKINS_HOME}
ls -a dockerbuild.sh
file dockerbuild.sh sh +x dockerbuild.sh'''
      }
    }
  }
  environment {
    JENKINS_HOME = '\'/opt/chams/simple-python-pyinstaller-app\''
  }
}