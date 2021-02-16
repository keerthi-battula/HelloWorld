pipeline {
agent any
  tools{
    maven 'MAVEN'
  }
stages {
stage ('bulid')
{
steps {
bat 'mvn -B -DskipTests clean'
}
}
stage ('test')
{
steps 
{
bat 'mvn test install'
}

}
}
}
