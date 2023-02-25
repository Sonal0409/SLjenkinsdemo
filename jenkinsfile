pipeline{
    
    tools{
        maven 'mymaven'
    }
    
    agent any
    
    stages{
        stage ('Clone a repo'){
            steps{
                git 'https://github.com/Sonal0409/DevOpsCodeDemo.git'
            }
        }
       stage('Compile Code') {
           steps{
               sh 'mvn compile'
           }
       }
       
       stage('Test'){
       steps{
           sh 'mvn test'
       }
       }
       
       stage('package'){
           steps{
               sh 'mvn package'
           }
       }
    }
}
