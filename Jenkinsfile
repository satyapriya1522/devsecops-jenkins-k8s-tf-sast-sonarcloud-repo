pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=udemybuggywebapp -Dsonar.organization=udemybuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=5527d4c08f562569fa644d76f57c182bba1a0316'
			}
        } 
  }
}
