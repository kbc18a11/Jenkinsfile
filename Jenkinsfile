
// https://www.jenkins.io/doc/pipeline/tour/tests-and-artifacts/をmaven対応させる
pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                dir('./my-app') {
                    sh 'cat pom.xml'
                    sh 'mvn install'
                    sh 'mvn package'
                }
            }
        }
    }
}
