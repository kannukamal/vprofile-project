pipeline {
    
	agent any
/*	
	tools {
        maven "maven3"
    }
*/	
    environment {
        SNAP_REPO = 'vprofile-snapshot'
        NEXUS_USER = 'admin'
        NEXUS_PASS = 'Kamal9737@'
        RELEASE_REPO = 'vprofile-release'
        CENTRAL_REPO = 'vpro-maven-central'
        NEXUS_VERSION = "nexus3"
        NEXUS_PROTOCOL = "http"
        NEXUSIP = "172.31.20.241"
        NEXUSPORT = '8081'
        NEXUS_GRP_REPO = 'vpro-maven-group'
        NEXUS_REPOSITORY = "vprofile-release"
	    NEXUS_REPOGRP_ID    = "vprofile-grp-repo"
        NEXUS_CREDENTIAL_ID = "nexuslogin"
        NEXUS_LOGIN = 'nexuslogin'
        ARTVERSION = "${env.BUILD_ID}"
    }
	
    stages{
        
        stage('BUILD'){
            steps {
                sh 'mvn -DskipTests install'
            }
          
        }

	


    }


}
