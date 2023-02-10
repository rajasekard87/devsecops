pipeline {
    agent any
    tools{
        maven 'maven-3.9.0'
    }
        stages{
            stage('git stage'){
                steps{
                    git branch: 'main', credentialsId: 'github-credentials', url: 'https://github.com/rajasekard87/devsecops'
                }
            }
          
            stage('build maven project'){
                steps{
                   sh 'mvn clean install'
                }
            }
        }
}
