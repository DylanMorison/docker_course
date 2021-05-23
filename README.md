# [The Complete Guide to Docker](https://www.udemy.com/course/docker-and-kubernetes-the-complete-guide/)

### Section 6: Creating a Production-Grade WorkFlow

How will we develop a workflow where we 
1. Develop
2. Test
3. Deploy

All the code we write in this section will be container in a github repo.  We will have two branches:
- **feature branch**: where code is pushed and pulled.
- **master branch**: changes here will be automatically deployed

the only way code enters master branch is through a PR from feature branch.  We will use `Travis CI` to test our changes and if the passes pass, automatically deploy them on AWS.

>Detailed Workflow:
1. **Development**
   1. make changes on feature branch
   2. push to github
   3. create PR to master branch
2. **Testing**
   1. Master branch + PR is sent to `Travis CI` for testing
   2. If tests pass merge PR to master.
3. **Production**
   1. Code pushed to Travis CI
   2. Tests run
   3. Deploy to AWS Elastic Beanstalk

But where does Docker come into play? Docker is simply a tool that makes executing this workflow *easier*. But it is not a requirement.

Commands:
```bash
docker build -f Dockerfile.dev .
```