# aws-lambda-jruby
Run ruby code on JRuby on AWS Lambda Java

### Now with serverless.yaml!

# How to use
1. Add your ruby code to src/main/resources/main.rb

2. Build project
```
./gradlew build
```
3. Crate AWS Lambda fuction on AWS

  put "AWSLambdaJRuby::handler" to handler setting


4. Upload zip file

  Zip file is created into build/distributions


5. Run Lambda function

  needs timeout of at least 60 sec for the first execution of the lambda
