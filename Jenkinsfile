pipeline {
    agent any
    stages {
        stage ('SCM') {
         steps {git 'https://github.com/devopsraja/pravin.lopes.git' }
        }
    stage ('Build') {
         steps { bat label: '', script: 'mvn clean'
                 bat label: '', script: 'mvn install'         }
        }
    stage ('deploy') {
         steps { bat label: '', script: 'xcopy /y "C:\\Program Files (x86)\\Jenkins\\workspace\\bujjububblu\\target\\jenifer.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps"'         }
        }
        
    }
}
