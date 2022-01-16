pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build....'
                git branch: 'master',
                    credentialsId: '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',
                    url: 'https://github.com/BlueVT1437/demo.git'

                sh '''
                ls -lat
                cd my-app
                sudo npm i
                npm start
                '''
                // git clone https://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@github.com/BlueVT1437/demo.git my-app
                // sudo npm i
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                // sh '''
                // npm install -g serve
                // serve -s build
                // '''
            }
        }
    }
}