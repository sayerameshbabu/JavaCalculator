pipeline{
  agent any
  environment{
    GITHUB=credentials('git')
    DOCKER=credentials('docker')
  }
  parameters{
    booleanParam(name:'executeTests',defaultValue:true, description:"enter true or false")
  }
  stages{
    stage("test.."){
      when{
        expression{
          params.executeTests
        }
      }
      steps{
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
