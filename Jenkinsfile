Pipeline {
    agent any
    tools {
        maven "MAVEN"
        jdk "jdk8"
    }

    environment{
        SNAP-REPO= 'tynybay-snapshot'
        RELEASE-REPO= 'tynybay-release'
        CENTRAL-REPO= 'tynybay-central'
        NEXUS-GRP-REPO= 'tynybay-group'
        NEXUS-USER= 'admin'
        NEXUS-PASS= '123'
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