pipeline{
    agent any{
        stages{

            stage("cleanup"){
                steps{
                deleteDir()
            }
            }

            stage("Checkout"){
                steps{
                    sh "git clone https://github.com"
                }
            }

            stage("Build"){
                steps{
                    dir("/simple-java-maven-app")
                    sh "mvn clean install"
                }
            }
        }
    }
}
