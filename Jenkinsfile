pipeline {
    
    agent any
    environment {
        TEST_VARIABLE = 'test'
    }
    stages {
        stage('copy') {
            steps{
                ssh 'ssk'
                /*
                withCredentials([]) {
                    //sh ‘ssh user@server mkdir -p /var/www/temp_deploy’
                    
                }*/
                echo 'End of Deployment'
            }
        }
    }
}