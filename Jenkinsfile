pipeline
{
agent any
stages
{
  stage('Build')
  {
    steps
    {
       bat 'echo %PATH%'
       echo env.PATH
    }
  }
  stage('Test')
  {
     steps
    {
        bat 'mvn test'
      echo 'basic test done'
     }
      steps
    {
      bat 'mvn integration-test'
      echo 'integration test done'
    }
   }
  stage('Verify')
  {
      bat 'mvn verify'
      echo 'verfication done'
  }
}
}
