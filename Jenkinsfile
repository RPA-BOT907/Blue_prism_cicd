pipeline {
    agent any

    stages {
        stage('Run Bat Commands') {
            steps {
                  bat 'echo "Hello, World!"'
                  def path1 = '\Program Files\Blue Prism Limited\Blue Prism Automate'
                  dir(path: path1, includeParent: false) {
                      env.path = 'C:\\Users\\haris\\Downloads\\BPA Process - pro.bpprocess'
                      env.username = 'admin'
                      env.password = 'Sarasu@10'
                      bat 'AutomateC.exe /importr "%path%" /user "%username%" "%password%"'
                      bat 'AutomateC.exe /publish "Pro" /user "%username%" "%password%"'
                  }
                  bat 'echo "completed successfully"' 
            }
        }
    }
}
