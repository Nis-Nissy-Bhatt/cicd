pipeline{
    agent any
    stages{
        stage("compile"){
            steps{
                bat 'javac Lion.java'
                 script: ''' @echo off
                            return_1_if_success.exe   // command which returns 1 in case of success, 0 otherwise
                            IF %ERRORLEVEL% EQU 1 (exit /B 0) ELSE (exit /B 1)'''
            }
        }
        stage("run"){
            steps{
                bat"java Lion"
            }
        }
    }
}