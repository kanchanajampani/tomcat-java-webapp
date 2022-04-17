pipeline {
    agent any

    tools {
        maven "maven35"
    }

    stages {
        stage('Build') {
            steps {
                // git 'https://github.com/stardomsolutions/tomcat-java-webapp.git'

                sh "mvn clean package"
            }
        }
		
    }
}
