pipeline {
  * agent any

    stages {

        *tage('Checkout') {
            ste*s {
                git*'https://github.com/govanya0428/cic*.git'
            }
        }

   *    stage('Build Docker Image') {
*           steps {
               *sh 'docker build -t mywebsite1 .'
 *          }
        }

        sta*e('Stop Old Container') {
        *   steps {
                sh 'doc*er rm -f mywebsite1 || true'
      *     }
        }

        stage('D*ploy Container') {
            ste*s {
                sh '''
       *        docker run -d \
          *     --name mywebsite1 \
          *     -p 8081:80 \
                *ywebsite1
                '''
     *      }
        }
    }
}
