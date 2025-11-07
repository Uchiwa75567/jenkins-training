pipeline {
    agent any
    environment {
        NOM = 'Ahmed'
    }
    stages {
        stage('Salut') {
            steps {
                sh 'echo "Salut $NOM"'  // ← GUILLEMETS OBLIGATOIRES
            }
        }
    }
}
