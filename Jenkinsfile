pipeline {
  agent any
  stages {
    stage('error') {
      agent any
      steps {
        bat(script: 'D:\\temp\\jenkins\\script.bat', label: 'list LW C', returnStatus: true, returnStdout: true)
      }
    }

  }
}