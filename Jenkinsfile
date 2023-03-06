pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/ysreddy1695/jenkins.git'

                // Run a Unix 
                // To run Maven on a Windows agent, use
                // bat "mvn -Dmaven.test.failure.ignore=true clean package"
            }   
        }
        stage('Maven Build') {
            sh "mvn clean package"
        }
    }
}
