pipeline{
    agent{
        docker{
            image "cypress/browsers:latest"
            args '--entrypoint='
        }
    }
    stages{
        stage('Hello'){
            steps{
                echo "hello from Jenkinsfile"
            }
        }
        stage('install dependances'){
            steps{
                sh "npm ci"
            }
        }
        stage('Run tests'){
            steps{
                sh "npx cypress run"
            }
        }
    }
}