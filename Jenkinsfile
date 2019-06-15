pipeline {
   agent any
   stages {

      stage ('Build') {
         when {
            branch 'master'
         }
         steps {
            sh "chmod +x gradlew"
            sh "./gradlew build publish --stacktrace"
         }
      }
   }
}
