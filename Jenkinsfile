node('master')
{
  stage('ContinuousDownload_Master') 
  {
    git 'https://github.com/intelliqittrainings/maven1.git'
  } 
  stage('ContinuousBuild_Master')
  {
      sh label: '', script: 'mvn package'
  }
    
    
    
    
    
    
}
