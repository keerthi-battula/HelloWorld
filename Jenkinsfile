pipeline {
agent any
  tools{
    maven 'Maven'
  }
stages {
stage ('bulid')
{
steps {
sh 'mvn -B -DskipTests clean package'
}
}
stage ('test')
{
steps 
{
sh 'mvn test'
}

}
}
}
