pipeline{
    agent any
    stages {
        stage (test) {
            steps {
                echo "hello world"
            }
        }
        stage (build) {
            agent {label "OPENJDK8-MVN11"}
            steps {
                git url: "https://github.com/spring-projects/spring-petclinic.git",
                branch: "main"
            }
        }
    }
}