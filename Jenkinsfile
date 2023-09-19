pipeline
{
agent any
stages
{
stage("checkout")
{
  steps
{
   git credentialsId: 'gitcredentials', url: 'https://github.com/hellotohello/springproject.git'
}
}
stage("compile")
{
  steps
  {
    bat "mvn compile"
  }
}
stage("test")
 {
   steps
{
   bat "mvn test"
}
}
stage("package")
 {
   steps
 {
    bat "mvn package"
 }
}
}
}
