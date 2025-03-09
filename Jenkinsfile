pipeline {
    agent { docker { image 'node:22.14.0-alpine3.21' } }
    stages {
        stage('Initialize'){
            def dockerHome = tool 'myDocker'
            env.PATH = "${dockerHome}/bin:${env.PATH}"
        }
        stage('build') {
            steps {
                sh 'node --version'
            }
        }
    }
}
