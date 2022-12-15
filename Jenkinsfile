pipeline {
    agent any
    
    stages {
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
