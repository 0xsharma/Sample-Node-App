pipeline {
    agent { label 'w62ecs' }
    
    stages {
        stage('deploy') { 
            steps {
                
                echo "lol2"
                sh "docker build -t samplenode ."
            }
        }
    }
}
