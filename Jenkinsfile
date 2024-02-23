pipeline{
    agent any
    environment{
        staging_server="103.192.198.221"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
                sh 'scp -r ${WORKSPACE}/* root@${staging_server}:/var/www/finaleap.in/test/'
            }
        }
    }
}
