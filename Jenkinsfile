pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                sleep(5)
                echo "Build 1"
                echo "Build 2"
                echo "Build 3"
                echo "Build 4"
            }
        }
        stage("Test") {
            steps {
                echo "Test Running 1"
                echo "Test Running 2"
                sleep(5)
                echo "Test Running 3"
                echo "Test Running 4"
            }
        }
        stage("Deploy") {
            steps {
                echo "Deploy Running 1"
                echo "Deploy Running 2"
                echo "Deploy Running 3"
                echo "Deploy Running 4"
                sleep(20)
                echo "Deploy Running 5"
            }
        }
    }
    post {
        always {
            echo "Always Condition"
        }
        success {
            echo "Jika sukses"
        }
        failure {
            echo "Gagal tol"
        }
        cleanup {
            echo "gapeduli sukses or gagal kamu tetap yang terbaik"
        }
    }
}