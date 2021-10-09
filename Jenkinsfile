pipleline
{
agent any
stages
{
    stage('scm checkout')
    { steps { git branch: 'master', url: 'https://github.com/itspri746/maven-project' } }

    stage('code build')
    { steps { withMaven(jdk: 'java_home', maven: 'maven_home') {
        sh 'mvn clean package'

}   }  }
    
}
}

