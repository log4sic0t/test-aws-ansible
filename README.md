STEPS FOLLOWED

- created a docker container (with ubuntu 22.04) on a internal vm running in kvm

- on that container installed awscli and ansible
- on awscli
   - aws configure
   - create-key-pair 
   - create-security-group
        - authorize-security-group-ingress on port 22
        - authorize-security-group-ingress on port 80
   - run istance using image-id ami-0aaa5410833273cfe (ubuntu 22.04)
- on ansible 
   - modified ansible/hosts file
   - created an ansible playbook
   - runned the ansible playbook on 13.41.203.155

- logged in ssh using the pem key
- tested via w3m the site was reacheable

http://13.41.203.155/
