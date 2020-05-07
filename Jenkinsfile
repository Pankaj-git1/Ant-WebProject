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
    Steps
    {
    withAnt(installation: 'Local_Ant', jdk: 'Local_Java') {
    sh 'ant init '
}
    }
  }
  
}
}
