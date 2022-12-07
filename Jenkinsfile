pipeline {
    agent any

    stages {
      stage('Git_Repo') {
        steps {
          git 'https://github.com/Justic-D/sdvps-materials.git'
          sh 'ls -la'
        }
      }
      stage('Проверка') {
        steps {
          echo 'Выполняем проверку работы'
        }
      }
      stage('Тестирование') {
        steps {
          sh '/usr/local/go/bin/go test .'
        }
      }
      stage('Docker_Build') {
        steps {
          sh 'docker build .'
        }
      }
    }
}
