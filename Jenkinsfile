pipeline {
agent any
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
