pipeline {
  agent { label 'generic' }

  stages {
    //stage('Build') {
      //steps {
        //echo 'Building...'
      //}
    //}
    stage('Test_Checkmarx') {
      steps {
        echo 'Testing Checkmarx...'
		step([$class: 'CxScanBuilder', comment: '', configAsCode: true, credentialsId: 'Checkmarx_Cred', customFields: '', excludeFolders: '', exclusionsSetting: 'global', failBuildOnNewResults: false, failBuildOnNewSeverity: 'HIGH', filterPattern: '''!**/_cvs/**/*, !**/.svn/**/*, !**/.hg/**/*, !**/.git/**/*, !**/.bzr/**/*,
        !**/.gitgnore/**/*, !**/.gradle/**/*, !**/.checkstyle/**/*, !**/.classpath/**/*, !**/bin/**/*,
        !**/obj/**/*, !**/backup/**/*, !**/.idea/**/*, !**/*.DS_Store, !**/*.ipr, !**/*.iws,
        !**/*.bak, !**/*.tmp, !**/*.aac, !**/*.aif, !**/*.iff, !**/*.m3u, !**/*.mid, !**/*.mp3,
        !**/*.mpa, !**/*.ra, !**/*.wav, !**/*.wma, !**/*.3g2, !**/*.3gp, !**/*.asf, !**/*.asx,
        !**/*.avi, !**/*.flv, !**/*.mov, !**/*.mp4, !**/*.mpg, !**/*.rm, !**/*.swf, !**/*.vob,
        !**/*.wmv, !**/*.bmp, !**/*.gif, !**/*.jpg, !**/*.png, !**/*.psd, !**/*.tif, !**/*.swf,
        !**/*.jar, !**/*.zip, !**/*.rar, !**/*.exe, !**/*.dll, !**/*.pdb, !**/*.7z, !**/*.gz,
        !**/*.tar.gz, !**/*.tar, !**/*.gz, !**/*.ahtm, !**/*.ahtml, !**/*.fhtml, !**/*.hdm,
        !**/*.hdml, !**/*.hsql, !**/*.ht, !**/*.hta, !**/*.htc, !**/*.htd, !**/*.war, !**/*.ear,
        !**/*.htmls, !**/*.ihtml, !**/*.mht, !**/*.mhtm, !**/*.mhtml, !**/*.ssi, !**/*.stm,
        !**/*.bin,!**/*.lock,!**/*.svg,!**/*.obj,
        !**/*.stml, !**/*.ttml, !**/*.txn, !**/*.xhtm, !**/*.xhtml, !**/*.class, !**/*.iml, !Checkmarx/Reports/*.*,
        !OSADependencies.json, !**/node_modules/**/*''', fullScanCycle: 10, generatePdfReport: true, groupId: '53', password: '{AQAAABAAAAAQmjNhbGgdCpMZP4oyrcwv38pEN1QExKMCWZ7TLlhmstw=}', preset: '36', projectName: 'Pipeline_Seguridad', sastEnabled: true, serverUrl: 'https://cxprivatecloud.checkmarx.net/', sourceEncoding: '6', useOwnServerCredentials: true, username: '', vulnerabilityThresholdResult: 'FAILURE', waitForResultsEnabled: true])
	  }
    }
	  //step([$class: 'CxScanBuilder', comment: '', credentialsId: 'cxprivatecloud.checkmarx.net', customFields: '', dependencyScanConfig: [dependencyScanExcludeFolders: '', dependencyScanPatterns: '', dependencyScannerType: 'SCA', enableScaResolver: 'MANIFEST', fsaVariables: '', osaArchiveIncludePatterns: '*.zip, *.war, *.ear, *.tgz', overrideGlobalConfig: true, pathToScaResolver: '', sastCredentialsId: '', scaAccessControlUrl: 'https://platform.checkmarx.net/', scaConfigFile: '', scaCredentialsId: '8f6aedf0-067a-4a33-8526-00660bed6125', scaEnvVariables: '', scaResolverAddParameters: '', scaSASTProjectFullPath: '', scaSASTProjectID: '', scaSastServerUrl: '', scaServerUrl: 'https://api-sca.checkmarx.net', scaTeamPath: '', scaTenant: 'Nfr_sca_kmhcorp', scaWebAppUrl: 'https://sca.scacheckmarx.com'], excludeFolders: '', exclusionsSetting: 'global', failBuildOnNewResults: false, failBuildOnNewSeverity: 'HIGH', filterPattern: '''!**/_cvs/**/*, !**/.svn/**/*, !**/.hg/**/*, !**/.git/**/*, !**/.bzr/**/*,
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
        //!OSADependencies.json, !**/node_modules/**/*''', fullScanCycle: 10, generatePdfReport: true, groupId: '53', password: '{AQAAABAAAAAQCziBTAqjWVQnFg+xdVcd46squYe6+fc1tfoEoTPY33w=}', preset: '36', projectName: 'Pipeline_Seguridad', sastEnabled: true, serverUrl: 'https://cxprivatecloud.checkmarx.net/', sourceEncoding: '6', useOwnServerCredentials: true, username: '', vulnerabilityThresholdResult: 'FAILURE', waitForResultsEnabled: true])
    //}
  //}  
    stage('Test_Kiuwan') {
      steps {
        echo 'Testing Kiuwan...'
	      kiuwan applicationName: 'PIPELINE_SEGURIDAD', connectionProfileUuid: '5PIH-WqhL', failureThreshold: 60.0, label: '00008', sourcePath: '/home/jenkins/jenkins_slave/workspace/Pipeline_Seguridad', unstableThreshold: 96.0
	  }
    }
	  
    stage('Test_Snyk_SCA') {
      steps {
        echo 'Testing Snyk SCA...'
        snykSecurity(
          snykInstallation: 'snyk@latest',
          snykTokenId: 'Id_Snyk_Cred',
	  failOnIssues: false,
	)
      }
    }
	
    stage('Test_Snyk_SAST') {
     steps {
        echo 'Testing Snyk SAST...'
        snykSecurity(
          snykInstallation: 'snyk@latest',
          snykTokenId: 'Id_Snyk_Cred',
	  additionalArguments: '--code',
	  failOnIssues: false,
	)
      }
    }
	  
    
    //stage('Deploy') {
      //steps {
        //echo 'Deploying...'
      //}
    //}
  }
}
