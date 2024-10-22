
// https://www.jenkins.io/doc/pipeline/tour/tests-and-artifacts/をmaven対応させる
pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn install'
                sh 'mvn package -f my-app'
            }
        }
    }
}
