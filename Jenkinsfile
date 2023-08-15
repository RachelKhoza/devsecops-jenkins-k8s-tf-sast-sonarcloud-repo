pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=thederiorg_derivorg_buggywebapp -Dsonar.organization=thederiorg -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=36af5d1f1b2868d11e7be4b0b377db8a80408eed'
			}
        } 
  }
}
