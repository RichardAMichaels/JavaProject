pipeline
{
  agent any
    stages
    {
        stage('Build')
        {
            steps
            {
                  sh 'ant -f build.xml -v'
            }
        }
    }
    post
    {
      always
      {
        archiveArtifacts  artfacts: 'dist/*.jar', fingerprint:true
      }
    }
}
