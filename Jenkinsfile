pipeline{
    agent{
        docker{
            image "cypress/browsers:latest"
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
                sh "npx cypress install"
            }
        }
        stage('Run tests'){
            steps{
                sh "npx cypress run"
            }
        }
    }
}