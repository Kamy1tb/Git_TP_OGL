pipeline {
  agent any
  stages {
    stage("test"){
      steps{
      bat 'gradlew test'
      junit 'build/test-results/test/*.xml' 
      cucumber buildStatus: 'UNSTABLE',
      reportTitle: 'My report',
      ileIncludePattern: 'target/report.json',
      }
    }
    
}

}
