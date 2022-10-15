pipeline { 
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                git 'https://github.com/s98765499/helloworld.cpp.git'
                sh 'g++ helloworld.cpp -o helloworld'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh './helloworld'
            }
        }
    }
}
