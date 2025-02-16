pipeline{
    agent any
    stages{
        stage('Restor Dependances'){
            steps{
                bat 'dotnet restore'
            }
        }
        stage('Build Project'){
            steps{
                bat 'dotnet build'
            }
        }
        stage('Run dotnet tests'){
            steps{
                bat 'dotnet test'
            }
        }
    }
}