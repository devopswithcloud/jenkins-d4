pipeline {
    agent any 
    tools {
        maven 'MAVEN_PATH' // this name should match the name under tools section in jenkins
    }
    stages {
        stage ('Maven') {
            steps {
                echo "***** Maven Version ******"
                sh 'mvn --version'
            }
        }
        stage ('SpecificStage') {
            steps {
                echo "****** Executing Tools under Stage area ******"
                sh "mvn --version"
            }
        }
    }
}
