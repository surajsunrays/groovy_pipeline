pipeline
{
    agent any
    stages
    {
        stage("checking branch")
        {
            steps
            {
                checkout scm
                script
                {
                    echo "Value of server is $server";
                }
            }
        }
    }
}
