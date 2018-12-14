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
                    sh 'git checkout test'
                    sh 'git branch'
                    
                }                              
                if("$server".matches("STAGE SERVER"))
                {
                    echo "APPLICATION WILL BE DEPLOYED TO STAGING SERVER";
                    sh 'git checkout stage'
                    sh 'git branch'
                }
                if("$server".matches("PRODUCTION SERVER"))
                {
                    echo "APPLICATION WILL BE DEPLOYED TO PRODUCTION SERVER";
                    sh 'git checkout prod'
                    sh 'git branch'
                }
                
            }
        }
    }
}
}
