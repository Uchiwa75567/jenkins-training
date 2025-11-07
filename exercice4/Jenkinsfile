pipeline{
    agent any
    stages{
        stage('Parallele'){
            stage('stage A'){steps{sh'sleep 5s;echo A ok'}}
            stage('stage B'){steps{sh'sleep 3s;echo B ok'}}
            }
        stage('Déployer'){
            input{message "Go prod?"}
            steps{
                echo'Déployé!'
            }
        }
        }


    }
