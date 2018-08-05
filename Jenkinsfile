pipeline
{
  agent any
    stages
    {
        stage('Build')
        {
            steps{
              step
              {
                  sh 'ant -f build.xml -v'
              }
            }
        }
    }
}
