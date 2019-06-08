pipeline {
    agent any
    stages {
        stage ("SCM"){
            steps {git 'https://github.com/joshmihi/hippo.git'}
        }
        stage ("BUILD"){
            steps {sh label: '', script: 'mvn clean'
   sh label: '', script: 'mvn install'}
        }
        stage ("DEPLOY"){
            steps { sh label: '', script: 'cp -rp "C:\\Program Files (x86)\\Jenkins\\workspace\\pipel\\target\\hippo.war" "C:\\Program Files (x86)\\Apache Software Foundation\\Tomcat 8.5\\webapps"'}
        }
    }
    
}
