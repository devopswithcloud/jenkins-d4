pipeline {
    agent any 
    tools {
        maven 'MAVEN_PATH' // this name should match the name under tools section in jenkins
    }
    stages {
        stage ('Maven') {
            steps {
                echo "***** Maven Version with default jave******"
                sh 'mvn --version'
            }
        }
        stage ('SpecificStage') {
            tools {
                jdk 'JDK-17'
            }
            steps {
                echo "****** Maven version with my custom java at /opt******"
                sh "mvn --version"
            }
        }
    }
}
