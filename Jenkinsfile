pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh "bash build.sh"
            }
        }
        stage('Test') {
            steps {
                sh "bash test.sh"
            }
        }
        stage('Deploy') {
            steps {
                sh 'cat ./deploy.sh'
                sh 'echo "Deploying..."'
                sh 'mv testfile.txt /tmp'
                sh 'ls -l /tmp'
            }
        }
    }
}
