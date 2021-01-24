pipeline {
    agent any 
    stages {
        stage('deploy') { 
            steps {
                
                bat "docker build -t samplenode ."
                bat "docker run --name dockerreact -p 80:3000 samplenode"
            }
        }
    }
}
