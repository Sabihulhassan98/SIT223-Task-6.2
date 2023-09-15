pipeline {
    agent any

    stages {
        stage("Build") {
            steps {
                // Use Maven as the build automation tool for example
                echo "Building with Mavendd"
            }
            post {
                always {
                    mail to: "sabihulhassan98@gmail.com",
                        subject: "Build Status Email",
                        body: "Build Successfull!"
                }
            }
        }

        stage("Unit and Integration Tests") {
            steps {
                echo "Running unit and integration tests ...."
            }
        }

        stage("Code Analysis") {
            steps {
                echo "Analyzing code ....."
            }
        }

        stage("Security Scan") {
            steps {
                echo "Performing security scan ......"
            }
        }

        stage("Deploy to Staging") {
            steps {
                echo "Deploying to staging server (e.g., AWS EC2 instance)"
            }
        }

        stage("Integration Tests on Staging") {
            steps {
                echo "Running integration tests on staging environment"
            }
        }

        stage("Deploy to Production") {
            steps {
                echo "Deploying to production server (e.g., AWS EC2 instance)"
            }
        }
    }
}
