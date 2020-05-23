node('master')
{
   stage('ContinuousDownload_master')
   {
      git 'https://github.com/SathyajithPuttaiah/maven.git'
   }
   stage('ContinuousBuild_master')
   {
       sh label: '', script: 'mvn package'
   }
   
}
