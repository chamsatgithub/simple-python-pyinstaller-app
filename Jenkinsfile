pipeline {
  agent {
    docker {
      image 'python:3.4-alpine'
      args '''ADD . /code
WORKDIR /code
RUN pip install -r requirements.txt
CMD ["python", "app.py"]

docker build -f /opt/chams/DockerFile . -t jenkintest:latest
docker run -it jenkintest'''
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