pipeline {
  agent any
    
    stages {
      stage ("Clone"){
        steps {
          git branch: 'main', url: 'https://github.com/Barada1/three-tier-app.git'
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
