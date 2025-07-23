# multipagewebsiteCICD
Denis personal multipage website CICD with githubactions


Overview Of what's required 

A GitHub repository with my personal website files (index.html, etc.)

An AWS S3 bucket already configured for static website hosting

An IAM user with access to that bucket (for GitHub Actions)

GitHub Actions workflow YAML file to deploy to the AWS S3 Bucket on push

Step 1 I created  an IAM user for Github Actions.
![alt text](<Bilder/Screenshot (237).png>)

![alt text](<Bilder/Screenshot (238).png>)


 Save the Access Key ID and Secret Access Key and we will save them on github later on.

 ![alt text](<Bilder/Screenshot (239).png>)

 Save the Access Key ID and Secret Access Key — you’ll need them in GitHub.

 2. Then add services to your Github Repo in your Github repository.
![alt text](<Bilder/Screenshot (240).png>)


Go to Settings > Secrets and variables > Actions > New repository secret

3. Then we Added a GitHub Actions Workflow File

![alt text](<Bilder/Screenshot (241).png>)

and a deploy.yml

![alt text](<Bilder/Screenshot (242).png>)


4. Test It
 We test the Github Acitions Pipeline by pushing changes made to the main branch
(e.g., edit a line in index.html)


Go to the Actions tab on GitHub → you’ll see the workflow running

![alt text](<Bilder/Screenshot (243).png>)

Visit your website — it should reflect the changes automatically!

Website changes reflected on S3 bucket and live website.


