pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('error') {
          agent any
          steps {
            bat(script: 'D:\\temp\\jenkins\\script.bat', label: 'list LW C', returnStatus: true, returnStdout: true)
          }
        }

        stage('test') {
          steps {
            zip(archive: true, zipFile: 'test.zip', dir: 'D:\\temp\\jenkins', overwrite: true)
          }
        }

      }
    }

  }
}