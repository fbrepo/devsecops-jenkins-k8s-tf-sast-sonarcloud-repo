pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=fbbuggywebapp -Dsonar.organization=fbBuggyWebApp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=218ee4731c9ef74dbac68e85fab7ef0c8dce2d1f'
			}
        } 
  }
}
