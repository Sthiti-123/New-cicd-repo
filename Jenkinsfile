pipeline {
       agent {
        node {
            label 'Jenkins-slave-Node'
        }
    }
 
    
    environment {
        PATH = "/opt/apache-maven-3.9.6/bin:$PATH"
    }
    stages {
        stage("Build Stage"){
            steps {
                echo "----------- build started ------------"
                sh 'mvn clean package -Dmaven.test.skip=true'
                echo "----------- build completed ----------"
            }
        }
       
    }
}
