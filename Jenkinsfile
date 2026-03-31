pipeline {
    agent any

    stages {

        stage('Install Newman') {
            steps {
                bat 'npm install -g newman'
            }
        }

        stage('Run API Tests') {
            steps {
                bat 'newman run api-testing/user-service-tests.postman_collection.json'
            }
        }

        stage('Generate Report') {
            steps {
                bat 'npx newman run api-testing/user-service-tests.postman_collection.json -r html --reporter-html-export newman/jenkins-report.html'
            }
        }

    }
}