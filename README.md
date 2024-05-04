# sgsummit24_sus_personalitytest
- Hosted on AppRunner (us-east-1-6583) https://tithebp62t.us-east-1.awsapprunner.com/ 
- After any update of files, rebuild with:
  - flutter build web
  - `docker build --platform=linux/amd64 -t sg-summit24-flutter-app .`
  - go to ECR to get push commands to the ECR repo (us-east-1-account-6583)
  - After pushing image, go to AppRunner and rebuild.
- Note about dockerizing
  - Dockerfile for details
  - in order to run it we also need a local server, which is responsible for assigning the port of the project where we run our image and starts the server to run the flutter image in a container.
  - `/server/server.sh`
  - ref: https://medium.com/@codemax120/flutter-web-with-docker-06cee1839adb

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

Ref:
https://medium.com/@codemax120/flutter-web-with-docker-06cee1839adb 