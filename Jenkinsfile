pipeline {
    agent any
    stages{
        stage('Build'){
            steps{
                bat 'npm install'
                script {
                    powershell '''
                        write-Output "Hello, World!"
                        $date = Get-Date
                        Write-Output "Current date and Time:$date"
                    '''
                }
                script{
                        powershell '''C:\\test-script\\myscript.ps1'''
                }
            }
        }

    }
}