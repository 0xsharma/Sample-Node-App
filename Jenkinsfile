pipeline {
    agent any 
    stages {
        stage('deploy') { 
            steps {
                
                bat "docker build -t samplenode ."
                bat "docker run --name samplenodecontainer -p 80:3000 samplenode"
            }
        }
    }
}
