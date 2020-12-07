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
        echo "${GITHUB_CREDENTIALS}"
      
        withCredentials([usernamePassword(credentialsId:'git',usernameVariable:USER,passwordVariable:PWD)]){
          echo "${USER}"
        
        }
      }
    }
  }
}
