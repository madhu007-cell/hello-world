pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('error') {
      steps {
        sh 'git clone https://github.com/madhu007-cell/hello-world.git'
        sh 'mvn clean package'
      }
    }

  }
}