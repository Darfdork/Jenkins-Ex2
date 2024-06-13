pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh "build.sh"
            }
        }
        stage('Test') {
            steps {
                sh ":test.sh"
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
