pipeline {
    agent any

    stages {
        stage('Run Bat Commands') {
            steps {
                  bat 'echo "Hello, World!"'
                 bat 'set path1="C:/Users/haris/Downloads/BPA Process - pro.bpprocess"'
                 bat  'cd %path1%'
                 bat 'set path="C:\Users\haris\Downloads\BPA Process - pro.bpprocess"'
                 bat 'set username="admin"'
                 bat 'set password="Sarasu@10"'
                 bat 'AutomateC.exe /importrelease %path% /user %username% %password%'
                 bat 'AutomateC.exe /publish "Pro" /user %username% %password%'
                 bat 'echo "completed successfully"' 
            }
        }
    }
}
