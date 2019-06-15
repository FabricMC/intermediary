pipeline {
   agent any
   stages {

      stage ('Build') {
         when {
            branch 'master'
         }
         steps {
            sh "rm -rf build/libs/"
            sh "chmod +x gradlew"
            sh "./gradlew build publish --stacktrace"
         }
      }
   }
}
