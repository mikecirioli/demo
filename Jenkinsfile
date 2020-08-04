pipeline {
agent  any
    stages {
      stage('CI Build and push snapshot') {
        when {
          branch 'PR-*'
        }
        steps {
          container('maven') {
            sh "mvn clean package"
          }

        }
      }
    }
  }
