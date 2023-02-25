# AzureDeployment
WebPage for tutorial "Deployment in Azure". This page I have used as HelloWorlAspNet

How to add your website in Bash step-by-step:

git clone "url adress of your git repository"

git config --global user.email "your email"

git config --global user.email "your name"

cd "path to your startup page(like index.html)"

git init

git add . 

git commit -m "Message"

az webapp deployment source config-local-git --name  "Name of your project" --resource-group "Name of your resource group"

az webapp deployment  list-publishing-credentials --name "Name of your project" --resource-group "Name of your resource group"

git remote add azure 'Link from "scmUri": (from generated JSON object)' //Because of $ your link has to be in '' quotation marks

