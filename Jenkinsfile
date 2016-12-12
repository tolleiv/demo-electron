node {
  checkout scm
  sh 'npm install'
  sh 'npm run build-linux'
  dir('dist') {
    archiveArtifacts artifacts: '*.AppImage', fingerprint: true;
  }
}
