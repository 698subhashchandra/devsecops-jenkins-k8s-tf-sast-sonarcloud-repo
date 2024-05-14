pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapplication -Dsonar.organization=asgbuggywebapplication -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=5102b2299f5bea2efd26f81510a1f4a2440d8a6e'
			}
        } 
  }
}
