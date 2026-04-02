All developers will work in the development branch/ test branch
- create sub branches

Then merge development branch into staging/ pre-production (use a copy of real-world data)

Then merge the staging branch to the main branch (production code)

Then push to production

Deployment
- when low utility (12am -4am) (server will be restarted)
- find developers who are available to work

Known isses/ known bugs
- not show stoppers
- super expensive to fix

CI/CD
- continuous integration and continuous deployment
- unit test cases if failed, then no commit
- deployment if all tests pass, push the code to to a branch

Scaling
- vertical: buying more powerful server
- horizontal: a lot of tiny servers (elasticity)

Cloud platform (elasticity) e.g. Amazon, Azure
- set threshold: 75% create a new copy of the server
- don't need to plan ahead how many servers to buy
- if traffic is less than so many, then delete the boxes
- buy according to location and proximity

Monolithic service
- all code is packed into a single package
- one application goes down, the entire application goes down

Miscroservice architexture
- entire functionality is going to be divided into several tiny services
advantages
1. parallel building--each service is independent
2. even if one service is down, others can keep running
3. easy scaling-- clone only one service (buy a smaller server)

Docker
- pocket sized virtual machine
- Kubernetes assign work to each docker