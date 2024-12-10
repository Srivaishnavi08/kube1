pipeline {
    agent any
    stages{
        stage('build'){
            steps{
                script{
                    bat 'docker build -t week9 .'
                    bat 'docker tag week9:latest vaishnavi517/week9:latest'
                    bat 'docker push vaishnavi517/week9:latest'
                }
            }
        }
        stage('tests'){
            steps{
                script{
                    echo 'tests'
                }
            }
        }
        stage('deploy'){
            steps{
                script{
                    
                    bat 'minikube delete'
                    bat 'minikube start'

                    
                }
            }
        }
