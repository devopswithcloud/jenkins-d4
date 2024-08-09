// Timeout 
pipeline {
    agent any 
    stages {
        stage ('TimeoutStage') {
            steps {
                timeout(time: 5, unit: 'SECONDS') {
                    echo "Sleeping for 60 Sec"
                    sleep 60
                    // manager apptroval
                }
            }
        }
    }
}
