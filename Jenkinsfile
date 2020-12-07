pipeline{
  agent any
  environment{
    GITHUB=credentials('git')
    DOCKER=credentials('docker')
  }
  parameters{
    booleanParam(name:'executeTests',defaultValue:true, description:"enter true or false")
    booleanParam(name:'executeCommand',defaultValue:false, description: 'enter true or false')
    string(name:'SAMEERA',defaultValue:'male',description:"enter the gender")
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
       when{
          expression{
            params.executeCommand
          }
        }
      steps{
       
        echo "building"
          
      
      }
    }
    stage("deploy.."){
      steps{
        echo "gender of sameera is: ${params.SAMEERA}"
        echo "deplying"
      }
    }
  }
}
