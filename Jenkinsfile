currentBuild.displayName = "Ant-pipeline-#"+currentBuild.number
pipeline
{
agent any
stages
{
stage('SCM checkout')
{
steps
{
git branch: 'master', url: 'https://github.com/Pankaj-git1/Ant-WebProject.git'
}
}
stage('Ant build')  
  {
    steps
    {
    withAnt(installation: 'Local_Ant', jdk: 'Local_Java') 
      {
    sh 'ant init '
}
    }
  }
  //stage('Deployment')
   //{
   //  steps
  //   {
  //   sshagent(['tomcat_Ant']) 
  //     {
   //      sh 'scp -o StrictHostKeyChecking=no */target/*.war ec2-user@3.89.196.242:/var/lib/tomcat/webapps/
    //     //sh 'scp -o StrictHostKeychecking=no */target/*.war ec2-user@3.83.121.64:/var/lib/tomcat/webapps 
      // }
   //  }
   //}
  
}
}
