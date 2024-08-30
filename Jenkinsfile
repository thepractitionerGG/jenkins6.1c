pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Running unit and integration tests...'
                
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Running code analysis...'
                
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Performing security scan...'
                
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Deploying to staging...'
                
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Running integration tests on staging...'
               
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Deploying to production...'
                
            }
        }
    }
    post {
        always {
            mail to: 'developer@example.com',
                 subject: "Pipeline Status: ${currentBuild.currentResult}",
                 body: "Pipeline has finished. Status: ${currentBuild.currentResult}",
                 attachLog: true
        }
    }
}
