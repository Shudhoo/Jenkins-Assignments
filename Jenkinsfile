pipeline {
    agent none
    triggers {
        githubPush()
    }
    stages {
        stage('test') {
        agent { label 'test-server'}
        steps {
            git branch: 'develop', url: 'https://github.com/Shudhoo/Jenkins-Assignments.git'
        }
        }
        stage('prod') {
        agent { label 'prod-server'}
        steps {
            git branch: 'develop', url: 'https://github.com/Shudhoo/Jenkins-Assignments.git'
        }
        }
    }
}
