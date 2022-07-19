pipeline {
  agent { label 'generic' }

  stages {
    //stage('Build') {
      //steps {
        //echo 'Building...'
      //}
    //}
    stage('Test_Snyk') {
      steps {
        echo 'Testing...'
        snykSecurity(
          snykInstallation: 'snyk@latest',
          snykTokenId: 'Id_Snyk_Cred',
		  
	)
      }
    }
	stage('Test_Kiuwan') {
      steps {
        echo 'Testing...'
		kiuwan connectionProfileUuid: '5PIH-WqhL',
			failureThreshold: 40.0,
			sourcePath: '/',
			unstableThreshold: 90.0
	  }
    }
    //stage('Deploy') {
      //steps {
        //echo 'Deploying...'
      //}
    //}
  }
}
