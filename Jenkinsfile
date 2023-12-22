pipeline
{
    agent any

    tools
    {
        //Maven installation
        maven "Maven_Home"
    }
    
    stages
    {
        stage('Build')
        {
            steps
            {
                //Git repository
                
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
