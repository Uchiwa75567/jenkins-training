pipeline{
    agent any

    stages{
        stage('Branche'){
            steps{
                script{
                    if(env.BRANCH_NAME='main'){
                        sh'echo"PROD READY"'
                    }
                    else{
                        sh'echo"DEV MODE"'
                    }
                }
            }
        }
    }
}