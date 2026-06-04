pipeline {
    agent any

    // On dit à Jenkins d'utiliser le NodeJS qu'on vient de configurer
    tools {
        nodejs 'NodeJS 18'
    }

    stages {
        stage('Installation') {
            steps {
                echo 'Installation des dépendances...'
                sh 'npm install' 
            }
        }
        stage('Tests') {
            steps {
                echo 'Vérification du code...'
                sh 'npm test' // N'oublie pas de configurer tes tests React
            }
        }
        stage('Déploiement') {
            steps {
                echo 'Déploiement réussi sur le serveur de production !'
            }
        }
    }
}