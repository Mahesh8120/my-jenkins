pipeline {
    agent {
       node {
           label 'AGENT'
        }
        
}
     environment { 
        greetings = 'hello jenkins'
     }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
        failure{
            echo 'this will run when pipeline is failed,used generally to send some alerts'
        }
        success{
            echo 'this will run when pipeline is success'
        }
    }

}