pipeline {
  agent any

   tools {
	maven "jenkin-maven"
         }


   stages {
	    stage('SCM') {
                 steps {
                      git 'https://github.com/ashwin1-dev/23-april-maven2.git'
                        }
                       }

            stage('Build') {
                   steps {
                           sh "mvn clean package"
                         }
                       }


            stage ('deploy') {
                   steps {
                           sh "sudo cp  /var/lib/jenkins/workspace/pipe3/target/vlc2.war  /usr/share/tomcat/webapps"
                         } 
                        }
           }
   }
                         
	       
