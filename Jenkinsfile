pipeline {
    agent any
    
    stages {
        stage('deploy') { 
            steps {
                
                echo "lol2"
                
                
                sh "aws ecr get-login-password --region us-east-2 | docker login --username AWS --password-stdin 701782360245.dkr.ecr.us-east-2.amazonaws.com"
                sh "docker build -t w62nodeapp ."
                sh "docker tag w62nodeapp:latest 701782360245.dkr.ecr.us-east-2.amazonaws.com/w62nodeapp:latest"
                sh "docker push 701782360245.dkr.ecr.us-east-2.amazonaws.com/w62nodeapp:latest"
                
                
                
                
                
            }
        }
    }
}
