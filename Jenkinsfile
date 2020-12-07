pipeline{
  agent any
  tools{
    maven 'Maven1'
  }
  parameters{
    string(name:'VAR2', defaultValue:'default', description:'variable2')
  }
  environment{
    ENV1='environment file'
  }
  stages{
    stage("build"){
      steps{
        sh "mvn clean install"
      }
      stage("testing"){
        steps{
          sh 'mvn clean test'
        }
      }
      stage("deploying"){
        steps{
          sh 'mvnclean package'
        }
      }
    }
  }
}
