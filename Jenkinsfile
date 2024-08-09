pipeline {
    agent {
        label 'java-agent-slave'
    }
    stages {
        stage ('Build') {
            steps {
                echo "This is the Stage for Building MVN app"
                // linux commands 
                sh 'hostname -i'
            }
        }
        stage ('ScriptedStage'){
            steps {
                echo "********Executing Scripted Stage*******"
                // write some custom code 
                script {
                    // define a variable 
                    def course = "k8sother"
                    if (course == "k8s") {
                        println("Thanks for enrolling into $course")
                    }
                    else 
                        println("Do learn k8s")
                    }
                    sleep 10 // SECONDS 
            }
        }
        // stage ("Sonar") {
        //     steps {
        //         echo "Executing Sonar Stage"
        //     }
        // }
    }
}
