// Declerative way
pipeline {
    agent any 
    stages {
        stage ('init') {
            steps {
                sh "terraform init" // refresh //plan //apply //destroy 
            }
        }
        stage ('Planning') {
            steps {
                sh "terraform plan"
            }
        }
        stage ('apply') {
            steps {
                sh "terraform apply --auto-approve"
            }
        }
        stage ('destroy') {
            steps {
                sh "terraform destroy --auto-approve"
            }
        }
    }
}