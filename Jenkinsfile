pipeline{
    agent any
    stages{
        stage('deploytodev'){
            steps{
                echo "Deploying in dev"
            }
        }
        stage('deploytoprod'){
            when{
                //branch name
                expression {BRANCH_NAME ==~ /(production|staging)/ }
            }
            steps{
                echo "deploying to prod"
            }
        }
    }
}
