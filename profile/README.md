Create automations (microservices) in Jupyter notebook and deploy them with the click of a button

Setup your environment using the [Bitswan automation server CLI](https://github.com/bitswan-space/bitswan-automation-server)

<img width="9300" height="3953" alt="image" src="https://github.com/user-attachments/assets/18b18729-8410-456c-be0a-952dafa796cb" />

Repositories:

- bitswan (open source BSD)
  - Contains the bitswan python library: what you get when you import bitswan in your jupyter notebook
  - Contains the bitswan compiler: Which compiles jupyter notebooks into microservices
- bitswan-automation-server (open source BSD)
  Orchestration system for bitswan workspaces and gitops runspaces
- bitswan-gitops (open source BSD)
   Orchestration system for bitswan microservices that operates within workspaces and runspaces
- bitswan-editor (%95 open source)
   Specialized instance of visual studio codeserver designed to help you build bitswan microservices in jupyter
- automation-operations-center (proprietary)
   Proprietary monitoring and management system for bitswan deployments
