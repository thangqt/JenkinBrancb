pipeline {
   agent {
        docker {
            image 'gradle:4.5-jdk8-alpine'
        }
    }
   stages {
      stage('Build') {
         steps {
            sh 'gradle clean build'
            sh 'gradle clean build'
            junit '**/target/surefire-reports/TEST-*.xml'
         }
      }

      stage('Deloy') {
         steps {
            echo "Deloy stagin"
         }
      }
   }
}
