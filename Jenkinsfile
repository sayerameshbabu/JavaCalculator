pipeline{
  agent any
  environment{
    GITHUB=credentials('git')
    DOCKER=credentials('docker')
  }
  parameters{
    booleanParam(name:'executeTests',defaultValue:true, description:"enter true or false")
  }
  }
  stages{
    stage("test.."){
      steps{
   //     withCredentials([
     //     usernamePassword(credentials:'docker', usernameVariable: USER), passwordVariable: PWD1
       // ]){
        //  echo "${PWD1}"
       // }
        echo "${GITHUB}"
        echo "${DOCKER}"
        echo "${executeTests}"
      }
    }
    stage("build.."){
      steps{
      echo "building"
      }
    }
    stage("deploy.."){
      steps{
      echo "deplying"
      }
    }
  }
}
