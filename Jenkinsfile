pipeline
{
    agent any
    
    stages
    {
        stage('compile')
        {
            steps
            {
                echo 'Compile stage'
            }
        }
        
        stage('Build')
        {
            steps
            {
                echo 'Build stage'
            }
        }
        
        stage('Test')
        {
            steps
            {
                echo 'Test stage'
            }
        }
    }
    
    post
    {
        always
        {
            emailext body: 'summary', subject: 'Pipeline status', to: 'kuttyspartan999@gmail.com'
        }
    }
}
