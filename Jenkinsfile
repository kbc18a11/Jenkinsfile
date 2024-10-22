
// https://www.jenkins.io/doc/pipeline/tour/tests-and-artifacts/をmaven対応させる
pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn install -f my-app'
                sh 'mvn package -f my-app'
            }
        }
    }
    post {
        always {
            recordIssues tools: [spotBugs()]
        }
    }
}
