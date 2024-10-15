pipeline{
    agent any
    stages{
        stage('Build Project'){
            steps{
               bat 'dotnet build'
            }
        }
        stage('Test'){
            steps{
                bat 'dotnet test'

            }
        }
        stage('Publish'){
            steps{
                bat 'dotnet publish -c Release -o ./publish'
            }
        }
    }
}