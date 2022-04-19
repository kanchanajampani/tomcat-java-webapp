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
	stage('Docker Build') {
            steps {
                sh "docker build -t 594897282097.dkr.ecr.us-east-1.amazonaws.com/jendolab"
            }
        }
	    stage('Docker push') {
            steps {
                sh "docker push 594897282097.dkr.ecr.us-east-1.amazonaws.com/jendolab"
            }
        }
    }
}
