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
                echo "Value of server is $server";
                if($server=='TEST SERVER')
                {
                    echo "YOU SELECTED TEST SERVER";
                }                              
                if($server=='STAGE SERVER')
                {
                    echo "YOU SELECTED STAGE SERVER";
                }
                if($server=='PRODUCTION SERVER')
                {
                    echo "YOU SELECTED PRODUCTION SERVER";
                }
            }
        }
    }
}
