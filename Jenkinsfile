pipeline{
    agent {
  label 'ansible'
}
    stages{
        stage('First'){
            steps{
                sh 'rm -rf vector-role'
                sh 'git clone https://github.com/nikmokrov/vector-role.git'
                sh 'cd vector-role'
                sh 'molecule test'
            }
        }
    }
}
