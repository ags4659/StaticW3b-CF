# StaticW3b-CF
This repo contains the info to create static website stack in cloud formation with cloud front distribution

## Website 
https://d7vq1cm9471d.cloudfront.net new project



# Requried Resourcces 
- aws account 
- text editor
- web site(html, css etc.)

#Instructions to Reproduce

-login into aws.
- create a bucket and upload cloudformation.yaml
- copy S3 url 
- navigate to cloud formation.
- click on create stack 
- Choose Amazon s3 url
- paste url copied before 
- next page 
- give a stack name 
- valid bucket name for S3 web hosting 
- under Stack Failure Options choose **Preserve successfully provisioned resources**
- click next and accept and create stack 
- once stack is created 
- you can find s3 bucket on s3 dashboard
- uploade index.html document

# verification
Navigate to cloudfront distibution dashboard
- you will find the distribution created by Cloud formation Stack.
- copy Distribution domain name 
- paste it in the browser.

## Troubleshoot
- if the url gives error 
- edit the distribution under orgins choose s3
- make sure it the orgin is pointing to your s3 Bucket created my cloud formation and hit save changes 
- it will take couple of minutes to deploy
- once the status is updated you can try again the same domain name 

## Documentation
- I have developed my personal portfolio website with simialr resources.
- https://thegiridhar.com/  
- we can use this stack for initations, small business static websites, 
- its as cheap as $1 - $2 per month plus domain 
- current https://d7vq1cm9471d.cloudfront.net is not redirected to any domain.
- we can edit the yaml document with R53 resoucres and certification manager fro SSL.

## Alternatives and future Improvements
- deploy manually creating and configuring resources. https://thegiridhar.com/  time consuming and repeative work load
- host with AWS Amplify with CI/CD best way (i will experment in the Future)
- if i have more time i will learn to deploy with aws amplify and explore other alternatives.
- use GO SDK automate the current process to  avoide GUI and error handling
-  better Frontend skills for production.

