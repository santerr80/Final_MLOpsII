pipeline {
    agent any

    stages {
        stage('Инициализация') {
            steps {
                sh 'pip3 install -r requirements.txt'
            }
        }
        stage('Запуск тестов') {
            steps {
                sh 'python3 test_main.py'
            }
        }
        stage('Запуск приложения') {
            steps {
                sh 'python3 main.py'
            }
        }
    }
}
