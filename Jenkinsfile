pipeline {
    agent any
    tools{
	jdk "myjava"
    }
    stages {
        stage('Compile') {
            steps {
                    echo "Compile the code"
                    sh "mvn Compile"
            }
        }
            
        stage('Testing') {
            steps {
                    echo "Testing the code"
                    sh "mvn test"
            }
        }
            
        stage('Build') {
            steps {
                    echo "Building the code"
                    sh "mvn package"
            }

        }
    }
}
