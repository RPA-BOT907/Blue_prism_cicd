pipeline {
    agent any
    stages {
        stage('Run Commands') {
            steps {
                bat 'echo "Hello, World!"'
                def path1 = '\\Program Files\\Blue Prism Limited\\Blue Prism Automate'
                bat "cd ${path1} && Automate.exe /import /file \"C:/Users/User1/Documents/Process1.xml\""
                bat 'echo "completed successfully"'
            }
        }
    }
}
