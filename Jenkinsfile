pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/GenkoPuhov0220/01-02-Student-Registry-App'
            }
        }
        
        stage('Restore Dependencies') {
            steps {
                script {
                    def projectDir = 'YourProjectFolder' // Change this to your actual project directory
                    bat "cd ${projectDir} && dotnet restore"
                }
            }
        }

        stage('Build Project') {
            steps {
                script {
                    bat "cd YourProjectFolder && dotnet build --no-restore"
                }
            }
        }

        stage('Run Tests') {
            steps {
                script {
                    bat "cd YourProjectFolder && dotnet test --no-build"
                }
            }
        }
    }
}
