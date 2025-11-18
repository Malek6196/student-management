pipeline {
    agent any

    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Malek6196/student-management'
            }
        }

        stage('Build with Maven') {
            steps {
                sh 'mvn clean install -DskipTests'
            }
        }
    }
}
