pipeline{
  agent any
  environment{
    GITHUB=credentials('git')
    DOCKER=credentials('docker')
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
