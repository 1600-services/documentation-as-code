## github pages: https://1600-services.github.io/documentation-as-code/

## overview

### This repository employs an action called updatePage.yml to convert the content of slides/README.md into index.html using the Marp tool. Subsequently, the composite action JamesIves/github-pages-deploy-action@v4 is utilized to create a new branch named gh_pages and deploy the index.html as a GitHub Page.

## Docker Image Build and Push:

### The repository also utilizes our composite action (1600-services/github-actions-template@master) to create a Docker image and push it to Docker Hub.

## Reusable Simple Workflow:

### Finally, a reusable simple workflow (1600-services/github-actions-template/.github/workflows/reusableWorkflow.yml@master) is implemented to execute a "Hello World" message, which can be customized using a variable.