node {
    def app

    stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */

        checkout scm
    }
  stage('SonarqubeScanning'){
      
         sh '''
	     /usr/local/bin/sonar-scanner -Dsonar.host.url= -Dsonar.login=4a925bed3202f13ae94e761d259bb7cf199a4fbc  -Dsonar.projectKey=salesforcesonar
	    '''
  }
}
