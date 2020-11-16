node{
        cleanWs()
    try{



        def imageName='172.30.1.1:5000/myproject/apache_jm20'

       
        stage('SERVICE - Git checkout'){
        git branch: branchName, url: "http://gitlab.example.com/pipeline_explog/explog.git"
        //git branch: branchName, url: "http://gitlab.example.com/pipeline_explog/lamp_k8s.git"
        }

      
       

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
