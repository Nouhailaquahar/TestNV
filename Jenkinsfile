pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Cette étape récupère le code depuis votre référentiel Git
                checkout scm
            }
        }
        stage('Afficher un message') {
            steps {
                // Cette étape affiche un message
                echo 'Ceci est un message de test.'
            }
        }
    }
}
