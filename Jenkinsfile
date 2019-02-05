pipeline {
  agent any
  stages {
    stage('Deploy CloudHub') { 
      environment {
        ANYPOINT_CREDENTIALS = credentials('455242a9-5f39-45b2-910c-adcca9ab55e3')
      }
      steps {
        'mvn deploy -P cloudhub -Dmule.version=4.1.1 -Danypoint.username=${ANYPOINT_CREDENTIALS_USR} -Danypoint.password=${ANYPOINT_CREDENTIALS_PSW}' 
      }
    }
  }
}