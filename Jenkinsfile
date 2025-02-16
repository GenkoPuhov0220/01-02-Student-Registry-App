pipeline {
    agent any

    stages {
        stage('NPM Install') {
            steps {
                bar 'npm install'
            }
        }
        stage('Run Integration tests') {
            steps {
                bar 'npm run test'
            }
        }
    }
}
