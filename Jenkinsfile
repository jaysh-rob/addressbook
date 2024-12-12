pipeline {
    agent any
    tools{
	jdk "Jvm"
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
