pipeline {
    agent any
    stages {
        stage('Lire fichier') {
            steps {
                script {
                    writeFile file: 'noms.txt', text: 'Ali\nSara\nKarim'
                    def lignes = readFile('noms.txt').split('\n')
                    for (nom in lignes) {
                        echo "Bonjour ${nom.trim()}"
                    }
                }
            }
        }
    }
}