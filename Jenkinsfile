pipeline {
agent {
docker
{
image 'maven:3-alpine'
args '-v/root/.m2:/root/.m2'
}
}
stages {
stage ('bulid')
{
steps {
sh 'mvn -f HelloWorld/pom.xml clean'
}
}
stage ('test')
{
steps 
{
 sh 'mvn -f HelloWorld/pom.xml test install'
}

}
}
}
