node('master')
{
  stage('ContinuousDownload-Loans') 
  {
    git 'https://github.com/intelliqittrainings/maven1.git'
  } 
  stage('ContinuousBuild-Loans')
  {
      sh label: '', script: 'mvn package'
  }
  stage('ContinuousDeployment-Loans')
  {
      sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war ubuntu@172.31.42.214:/var/lib/tomcat8/webapps/qaapp.war'
  }
  }
