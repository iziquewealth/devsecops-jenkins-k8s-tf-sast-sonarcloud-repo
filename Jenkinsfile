pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sonaropscloudasgbuggywebapp -Dsonar.organization=sonarOpsasgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login='8a391c537424e55de589f9a8fe9d2b3c0cdaef1e'
			}
        } 
  }
}
