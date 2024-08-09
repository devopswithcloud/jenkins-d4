pipeline {
    agent any 
    stages {
        stage ('Build'){
            steps {
                echo "****** Entering Build BLock ********"
                retry(3) {
                    echo "Welcome to D4"
                    error "Testing the retry block"
                }
                echo "****** After 3 retrys *******"
            }
        }
    }
}
