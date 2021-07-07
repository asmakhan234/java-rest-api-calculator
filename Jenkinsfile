pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                //git 'https://github.com/SHOAIBAHMED12842/java-rest-api-calculator.git'
                sh './mvnw clean compile'
                // bat '.\\mvnw clean compile'
            }
        }
        stage('Test') {
            steps {
                sh './mvnw test'
                // bat '.\\mvnw test'
            }

            post {
                always {
                    junit '**/target/surefire-reports/TEST-*.xml'
                }
            }
        }
    }
}
