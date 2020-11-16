node{
        cleanWs()
    try{

    
        stage('LANCEMENT DU DOCKER COMPOSE'){
        sh "docker-compose up -d"
        sh "docker ps"
       }


        stage('ARRET DU DOCKER COMPOSE'){
        sh "docker-compose down"
        sh "docker ps"
        }


        stage('FIN'){
            sh "echo 'FIN A BIENTOT !!!!'"
        }

    }
    finally{
        cleanWs()

    }
}
