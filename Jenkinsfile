node('master')
{
   stage('ContinuousDownload-Master1') 
   {
       git 'https://github.com/intelliqittrainings/maven.git'
   }
   stage('ContinuousBuild-Master1') 
   {
       sh label: '', script: 'mvn package'
   }

}
