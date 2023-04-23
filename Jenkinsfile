pipeline
{
  agent any
  stages
  {
    stages('Build')
    {
      steps
      {
        echo 'Build App'
      }
    }
    stages('Test')
    {
      steps
      {
        echo 'Test App'
      }
    }
    stage('Deploy')
    {
      steps
      {
        echo 'Deploy App'
      }
    }
  }
  Post 
  {
    failure
    {
      emailext body: 'Summary', subject: 'Pipline Status', to: 'keerthigganiga@gmail.com'
    }
  }
}
}
