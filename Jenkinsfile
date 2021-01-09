
node
{
   stage('cloning code')
    {
      git 'https://github.com/wakaleo/game-of-life.git'
    }
   stage('creating arfifacts')
   {
     sh 'mvn package'
   }
}


