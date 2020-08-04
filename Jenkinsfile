pipeline {
agent  any
    stages {
      stage('CI Build and push snapshot') {
        when {
          branch 'PR-*'
        }
        steps {
            sh "mvn clean package"
          }

        }
      }
    }
  }
