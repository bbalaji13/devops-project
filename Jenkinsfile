Pipeline {
    agent any
    tools {
        maven "MAVEN"
        jdk "jdk8"
    }

    environment{
        SNAP_REPO= 'tynybay-snapshot'
        RELEASE_REPO= 'tynybay-release'
        CENTRAL_REPO= 'tynybay-central'
        NEXUS_GRP_REPO= 'tynybay-group'
        NEXUS_USER= 'admin'
        NEXUS_PASS= '123'
        NEXUSIP= '172.31.17.97'
        NEXUSPORT= '8081'
        NEXUS_LOGIN= 'nexus-id' 
    }


    stages {
        stage('Build') {
            steps {
                sh 'mvn -s settings.xml -DskipTests install'
            }

        }
    }
}