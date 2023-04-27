pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
	maven 'maven'
    }
   

    stages{
        stage('build-the-app'){
            steps{
                echo 'this is the compile job'
                sh 'mvn compile'
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'mvn test'
            }
        }
        stage('three'){
            steps{
                echo 'this is the package job'
                sh 'mvn package'
            }
        }
    }
    
    post{
        always{
            echo 'hey! shopping-carts pipeline has completed...'
        }
        
    }
    
}
