node('master')
{
   stage('ContinuousDownload_loans')
   {
      git 'https://github.com/SathyajithPuttaiah/maven.git'
   }
   stage('ContinuousBuild_loans')
   {
       sh label: '', script: 'mvn package'
   }
   stage('ContinuousDeployment_loans')
   {
       sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war ubuntu@172.31.31.15:/var/lib/tomcat8/webapps/testapp.war'
       
   }
   
}
