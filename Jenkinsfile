pipeline {
    agent any

    stages {
        stage ('GetProject') {
            steps {
                git 'https://github.com/takfarinassaber/CT5171_springboot.git'
            }
        }
        stage ('build') {
            steps {
                sh 'mvn clean'

            }
        }
        stage ('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}