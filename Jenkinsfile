pipeline{
  agent any
  environment{
    GITHUB_CREDENTIALS=credentials('git')
  }
  tools{
    maven 'Maven1'
  }
  
  stages{
    stage("build"){
      steps{
        echo"${GITHUB_CREDENTIALS}"
      }
    }
  }
}
