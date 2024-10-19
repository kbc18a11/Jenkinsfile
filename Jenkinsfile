pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'echo ABC'
                timeout(time: 1, unit: 'MINUTES') {
                    echo(message: 'やくざ')
                }
            }
        }
    }
}
