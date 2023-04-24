pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=udemybuggywebapp -Dsonar.organization=udemybuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=e49943cb82dc133a5156c3d3d574d4afca7f05ac'
			}
        } 
  }
}
