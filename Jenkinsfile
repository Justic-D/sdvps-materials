pipeline {
 agent any
 stages {
  stage('Git') {
   steps {git 'https://github.com/Justic-D/sdvps-materials.git'}
  }
  stage('Test') {
   steps {
    sh 'go test .'
   }
  }
  stage('Build') {
   steps {
    sh 'docker build .'
   }
  }
  }
}
