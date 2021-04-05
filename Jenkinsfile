node
{
   stage('scm')
    {
       git 'https://github.com/wakaleo/game-of-life.git'
    }
   stage('mvn package')
   {
      sh 'mvn package'
   }
    stage('archiving artifacts')
     {
        archiveArtifacts artifacts: 'gameoflife-web/target/*.war', followSymlinks: false
     }
   stage('test reports')
    {
      junit '/scriptedtest-2/gameoflife-web/target/surefire-reports/*.xml'
    }
      
}
