pipeline {
  agent { label 'generic' }

  stages {
    //stage('Build') {
      //steps {
        //echo 'Building...'
      //}
    //}
    //stage('Test_Checkmarx') {
      //steps {
        //echo 'Testing Checkmarx...'
		//step([$class: 'CxScanBuilder', comment: '', configAsCode: true, credentialsId: 'Checkmarx_Cred', customFields: '', excludeFolders: '', exclusionsSetting: 'global', failBuildOnNewResults: false, failBuildOnNewSeverity: 'HIGH', filterPattern: '''!**/_cvs/**/*, !**/.svn/**/*, !**/.hg/**/*, !**/.git/**/*, !**/.bzr/**/*,
        //!**/.gitgnore/**/*, !**/.gradle/**/*, !**/.checkstyle/**/*, !**/.classpath/**/*, !**/bin/**/*,
        //!**/obj/**/*, !**/backup/**/*, !**/.idea/**/*, !**/*.DS_Store, !**/*.ipr, !**/*.iws,
        //!**/*.bak, !**/*.tmp, !**/*.aac, !**/*.aif, !**/*.iff, !**/*.m3u, !**/*.mid, !**/*.mp3,
        //!**/*.mpa, !**/*.ra, !**/*.wav, !**/*.wma, !**/*.3g2, !**/*.3gp, !**/*.asf, !**/*.asx,
        //!**/*.avi, !**/*.flv, !**/*.mov, !**/*.mp4, !**/*.mpg, !**/*.rm, !**/*.swf, !**/*.vob,
        //!**/*.wmv, !**/*.bmp, !**/*.gif, !**/*.jpg, !**/*.png, !**/*.psd, !**/*.tif, !**/*.swf,
        //!**/*.jar, !**/*.zip, !**/*.rar, !**/*.exe, !**/*.dll, !**/*.pdb, !**/*.7z, !**/*.gz,
        //!**/*.tar.gz, !**/*.tar, !**/*.gz, !**/*.ahtm, !**/*.ahtml, !**/*.fhtml, !**/*.hdm,
        //!**/*.hdml, !**/*.hsql, !**/*.ht, !**/*.hta, !**/*.htc, !**/*.htd, !**/*.war, !**/*.ear,
        //!**/*.htmls, !**/*.ihtml, !**/*.mht, !**/*.mhtm, !**/*.mhtml, !**/*.ssi, !**/*.stm,
        //!**/*.bin,!**/*.lock,!**/*.svg,!**/*.obj,
        //!**/*.stml, !**/*.ttml, !**/*.txn, !**/*.xhtm, !**/*.xhtml, !**/*.class, !**/*.iml, !Checkmarx/Reports/*.*,
        //!OSADependencies.json, !**/node_modules/**/*''', fullScanCycle: 10, generatePdfReport: true, groupId: '53', password: '{AQAAABAAAAAQmjNhbGgdCpMZP4oyrcwv38pEN1QExKMCWZ7TLlhmstw=}', preset: '36', projectName: 'Pipeline_Seguridad', sastEnabled: true, serverUrl: 'https://cxprivatecloud.checkmarx.net/', sourceEncoding: '6', useOwnServerCredentials: true, username: '', vulnerabilityThresholdResult: 'FAILURE', waitForResultsEnabled: true])
	  //}
    //}
	  
    stage('Test_Kiuwan') {
      steps {
        echo 'Testing Kiuwan...'
	      kiuwan applicationName: 'PIPELINE_SEGURIDAD', connectionProfileUuid: '5PIH-WqhL', excludes: '**/src/test/**,**/__MACOSX/**,**/*.min.js,**/*.Designer.vb,**/*.designer.vb,**/*Reference.vb,**/*Service.vb,**/*Silverlight.vb,**/*.Designer.cs,**/*.designer.cs,**/*Reference.cs,**/*Service.cs,**/*Silverlight.cs,**/.*,**/Pods/BuildHeaders/**/*.h,**/Pods/Headers/**/*.h,**/node_modules/**,**/bower_components/**,**/target/**,**/bin/**,**/obj/**,**/dist/**,**/lib/**,**/dev/shm/eic-hostkey-hjihi6wV**,**/etc/dhcp**,**/etc/grub.d**,**/etc/pki/CA/private**', failureThreshold: 96.0, label: '', sourcePath: '/', unstableThreshold: 97.0
	  }
    }
	  
    //stage('Test_Snyk') {
      //steps {
        //echo 'Testing Snyk...'
        //snykSecurity(
          //snykInstallation: 'snyk@latest',
          //snykTokenId: 'Id_Snyk_Cred',
	//)
      //}
    //}
	  
    
    //stage('Deploy') {
      //steps {
        //echo 'Deploying...'
      //}
    //}
  }
}
