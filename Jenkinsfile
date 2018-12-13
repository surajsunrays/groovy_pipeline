pipeline
{
    stages
    {
        stage("checking branch")
        {
            stapes
            {
                checkout scm
                script
                {
                    if($server="TEST SERVER")
                    git checkout test
                    else if($server="STAGE SERVER")
                    git checkout stage
                    else if($server="PRODUCTION SERVER")
                    git checkout prod
                }
            }
        }
    }
}