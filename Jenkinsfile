pipeline {
    agent any
    
    stages {
           stage("Clone Git Repository") {
            steps {
                git(
                    url: "https://github.com/Nouhailaquahar/TestNV.git",
                    branch: "main",
                    changelog: true,
                    poll: true
                )
            }
        }
        stage('Afficher Bonjour') {
            steps {
                echo 'Bonjour'
            }
        }
    }
}
