pipeline{
    agent any
    environment{
        DEPLOY_TO = 'production'
    }
    stages{
        stage('DeployProduction'){
            when{
                environment name :'DEPLOY_TO' , value:'production'
            }
            steps{
                echo " deploying the production env"
            }
        }
    }
}
