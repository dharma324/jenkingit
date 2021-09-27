pipeline 
{
    agent any

    stages
    {
        stage('build')
        {
            steps
            {
                echo 'build application'
            }
        }
        stage('test')
        {
            steps
            {
                echo 'test application'
            }
        }
        stage('deploy')
        {
            steps 
            {
                echo 'deploy application successfully'
            }
        }
    }
    post
    {
        always
        {
            emailext body: 'summary', subject: 'pipeline status', to: 'devops324@gmail.com'
        }
    }
}
