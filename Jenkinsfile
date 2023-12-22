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
                git 'https://github.com/kutty27/Maven-Project.git'

                //Run maven comnd
                bat "mvn -Dmaven.test.failure.ignore=true clean package"
                
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
