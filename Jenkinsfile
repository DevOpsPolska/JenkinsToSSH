pipeline {
    
    agent any
    environment {
        URI = 'test.local'

    }
    stages {
        stage('copy') {
            steps{
                sshagent (credentials: ['sshjanka']) {
                    $echo '$Username'
                    sh 'ssh-add -l'
                    sh 'ssh -o StrictHostKeyChecking=no -l $USERNAME $URI uname -a'
                }

                /*
                withCredentials([]) {
                    //sh ‘ssh user@server mkdir -p /var/www/temp_deploy’
                    
                }*/
                echo 'End of Deployment'
            }
        }
    }
}