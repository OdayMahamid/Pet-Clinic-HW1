
pipeline {
agent {label 'slave'}
tools{
maven 'MAVEN'
}
stages {
stage('clone') {
steps {
echo 'clone the repo'
git branch: 'main', credentialsId: '8a41edd1-54d5-4a79-b67e-66494b7a0134', url: 'https://github.com/spring-projects/spring-petclinic'

}
}
stage('build'){
steps{
dir('spring-petclinic'){
sh 'pwd'
}
script{'./mvnw package'}
}
}
}


