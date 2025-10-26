pipeline {
    agent any

    stages {
        stage('Build .NET project') {
            steps {
                sh 'dotnet build'
            }
        }
        stage('Test Unit and Integration tests') {
            steps {
                sh 'dotnet test --no-build --verbosity normal'
            }
        }
    }
}