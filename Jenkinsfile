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
                if("$server".matches("TEST SERVER"))
                {
                    echo "APPLICATION WILL BE DEPLOYED TO TEST SERVER";
                    git checkout test
                    git branch
                    echo "Current branch is :${BRANCH_NAME}";
                }                              
                if("$server".matches("STAGE SERVER"))
                {
                    echo "YOU SELECTED STAGE SERVER";
                }
                if("$server".matches("PRODUCTION SERVER"))
                {
                    echo "YOU SELECTED PRODUCTION SERVER";
                }
                
            }
        }
    }
}
}
