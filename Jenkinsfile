pipeline
{
    stages
    {
        stage("checking branch")
        {
           steps
           {
               if(env.server=='TEST SERVER')
                    echo "SELECTION IS TEST SERVER"
                else if(env.server=='STAGE SERVER')
                    echo "SELECTION IS STAGE SERVER"
                else if(env.server=="PRODUCTION SERVER")
                    echo "SELECTION IS PRODUCTION SERVER"
           }
        }
    }
}