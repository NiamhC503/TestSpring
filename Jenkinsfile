pipeline {
    agent any

    stages {
        stage ('GetProject') {
            steps {
                git 'https://github.com/NiamhC503/TestSpring.git'
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
        stage ('Archive') {
            steps {
                archiveArtifacts allowEmptyArchive: true,
                    artifacts: '**/demo*.war'
            }
        }
        stage ('Deploy') {
            steps {
                sh 'docker build -f Dockerfile -t myapp . '
                sh 'docker run --name "myappcontainer" -p 8081:8080 --detach myapp:latest'
            }
        }
    }
}