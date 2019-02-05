pipeline {
  agent any
  stages {
    stage('Deploy CloudHub') { 
      steps {
        sh 'mvn deploy -P cloudhub -Dmule.version=4.1.4 -Danypoint.username=${ANYPOINT_CREDENTIALS_USR} -Danypoint.password=${ANYPOINT_CREDENTIALS_PSW}' 
      }
    }
  }
}