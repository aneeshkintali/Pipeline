node('master')
{
   stage('ContinuousDownload-Master') 
   {
       git 'https://github.com/intelliqittrainings/maven.git'
   }
   stage('ContinuousBuild-Master') 
   {
       sh label: '', script: 'mvn package'
   }
<<<<<<< HEAD
=======
    stage('ContinuousDeployment') 
   {
       sh label: '', script: '''
scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war ubuntu@172.31.9.247:/var/lib/tomcat8/webapps/testapp.war'''
   }
   stage('ContinuousTesting')
   {
       git 'https://github.com/intelliqittrainings/FunctionalTesting.git'
   
       sh label: '', script: 'java -jar /home/ubuntu/.jenkins/workspace/ScriptedPipeline/testing.jar'
   }
   stage('ContinuousDelivery')
   {
        sh label: '', script: '''
scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war ubuntu@172.31.11.166:/var/lib/tomcat8/webapps/prodapp.war'''
   }
   
>>>>>>> 2d9883fb697de7aa801c8caa44e83b796d22af57
}
