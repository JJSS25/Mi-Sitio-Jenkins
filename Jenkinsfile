pipeline {
    agent any
    stages {
        stage('1. Clonar Código') {
            steps {
                echo 'Obteniendo el código más reciente desde GitHub...'
                git url: 'https://github.com/JJSS25/Mi-Sitio-Jenkins.git', branch: 'main'
            }
        }
        stage('2. Desplegar en Servidor Web') {
            steps {
                echo 'Copiando archivos al servidor Nginx...'
                sh 'cp -f *.html /var/website-data/'
            }
        }
    }
}
