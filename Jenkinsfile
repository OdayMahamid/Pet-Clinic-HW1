pipeline {
    agent {label 'slave'}//to run on jenkins slave
    tools{
        maven 'MAVEN'
    }
    stages {
        stage('clone') {
            steps {
         git branch: 'main', url: 'https://github.com/spring-projects/spring-petclinic.git'
}
}
       stage('build'){
           steps{
          
                  "./mvnw package"//build the app
           }
       }
}
}
