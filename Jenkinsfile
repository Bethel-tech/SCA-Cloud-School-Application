pipeline {
    agent any

    stages {

        stage('Build') 
        {
            steps 
            {
                echo 'Building stage'
            }
        }

         stage('Test') 
        {
            steps 
            {
                echo 'Testing stage'
            }
        }
         stage('Deploy') 
        {
            steps 
            {
                echo 'Deployment stage'
            }
        }
    }
    
    post
    {
        always
        {
           emailext body: 'The build job was successful', subject: 'Jenkins build', to: 'bethelosahon@gmail.com' 
        }
    }
}
