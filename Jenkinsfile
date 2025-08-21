pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Début du build...'
            }
        }
        stage('Test') {
            steps {
                script {
                    if (fileExists('index.html')) {
                        echo 'Le fichier index.html existe ✅'
                    } else {
                        error 'Le fichier index.html est manquant ❌'
                    }
                }
            }
        }
    }
}
