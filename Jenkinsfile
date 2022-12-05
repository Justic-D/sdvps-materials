pipeline {
 agent any
 stages {
  stage('Git') {
   steps {git 'https://github.com/Justic-D/sdvps-materials.git'}
  }
  stage('Test') {
   steps {
    sh '/usr/local/go/bin/go test .'
   }
  }
  stage('Build') {
   steps {
    sh 'docker build .'
   }
  }
 }
}