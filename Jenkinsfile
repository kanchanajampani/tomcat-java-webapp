pipeline {
    agent any

    tools {
        maven "maven35"
    }

    stages {
        stage('Build') {
            steps {
                sh "mvn clean package"
            }
        }
		
    }
}
