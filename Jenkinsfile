pipeline {
    agent any 
    stages {
        stage('deploy') { 
            steps {
                
                bat "docker build -t Sample-Node-App ."
                bat "docker run --name dockerreact -p 80:3000 Sample-Node-App"
            }
        }
    }
}
