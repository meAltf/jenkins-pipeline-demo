pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Read and Print File') {
            steps {
                script {
                    def content = readFile('test.txt')
                    echo "✅ Content of text.txt:"
                    echo content
                }
            }
        }

        stage('Custom Message') {
            steps {
                echo "🎉 Hey Alataf, you nailed it! Both files worked in one build."
            }
        }
    }
}
