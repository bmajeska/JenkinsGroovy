node('DOTNETCORE') {
    stage('SCM') {
    	echo 'Gathering code from version control'
        git branch: '${branch}', url: 'https://github.com/bmajeska/JenkinsGroovy.git'
    }
    stage('Build') {
        echo 'Building....'
        sh 'dotnet --version'
        sh 'dotnet build ConsoleApp1'
        echo 'Building New Feature'
    }
    stage('Test') {
        echo 'Testing....'
    }
    stage('Deploy') {
        echo 'Deploying....'
    }
}
