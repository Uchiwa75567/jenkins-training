pipeline {
    agent any

    stages {
        stage('Parallèle') {
            parallel {
                stage('Tâche A') {
                    steps {
                        sh 'sleep 5 && echo "A OK"'
                    }
                }
                stage('Tâche B') {
                    steps {
                        sh 'sleep 3 && echo "B OK"'
                    }
                }
            }
        }

        stage('Déployer ?') {
            input {
                message "Go prod ?"
                ok "Oui, déployer !"
            }
            steps {
                echo 'DÉPLOYÉ EN PROD !'
            }
        }
    }
}
