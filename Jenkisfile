pipeline {
  agent any
    
    stages {
      stage ("Clone"){
        steps {
          git "https://github.com/Barada1/three-tier-app.git"

        }
      }  
      
      stage ("Buid docker image") {
        steps {
          sh 'docker build -t myapp:latest .'

        }

      }
      
      stage ("Success") {
        steps {
          echo "Buid Success"

        }

      }

    }

}
