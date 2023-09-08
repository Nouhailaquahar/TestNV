
pipeline {
    agent any

    stages {
        stage('Cloner le référentiel') {
            steps {
                // Clonez le référentiel Git dans le workspace de Jenkins
                checkout scm
            }
        }

        stage('Installation des dépendances') {
            steps {
                // Installez les dépendances du projet Angular
                sh 'npm install'
            }
        }

        stage('Construction du projet') {
            steps {
                // Construisez le projet Angular
                sh 'ng build --prod'
            }
        }

        stage('Déploiement') {
            steps {
                // Copiez les fichiers de construction dans un répertoire de déploiement (par exemple, Apache, Nginx, etc.)
                sh 'cp -r dist/* /var/www/html'
            }
        }
    }
}
