pipeline{
    agent {
  label 'ansible'
}
    stages{
        stage('Git clone'){
            steps{
                git branch: 'main', url: 'https://github.com/nikmokrov/vector-role.git'
            }
        }
        stage('Run molecule test'){
            steps{
                sh 'molecule test'
            }
        }

    }
}
