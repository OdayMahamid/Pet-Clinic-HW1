pipeline {
    agent {label 'slave'}//to run on jenkins slave
    tools{
        maven 'MAVEN'
    }
    stages {
        stage('clone') {
            steps {
                echo 'clone the repo'
                git branch: 'main', credentialsId: '8a41edd1-54d5-4a79-b67e-66494b7a0134', url: 'https://github.com/spring-projects/spring-petclinic'
//extract from pipeline syntax
}
}
       stage('build'){
           steps{
                 dir('spring-petclinic'){// is same ass cd spring-petclinic
                   sh 'pwd'
               }
                 script{'./mvnw package'}//build the app
           }
       }
}
}
