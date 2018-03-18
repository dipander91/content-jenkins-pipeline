pipeline {
 agent any
 stages {
 stage('build') {
 steps {
sh 'echo "I am in build step"'
 sh 'javac -d . src/*.java'
 sh 'echo Main-Class: Rectangulator > MANIFEST.MF'
 sh 'jar -cvmf MANIFEST.MF rectangle.jar *.class'
 }
 }
 }
}
