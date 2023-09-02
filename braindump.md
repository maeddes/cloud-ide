Walkthrough:

Title
About me

Why? Reason for this talk - scenario at lecture

Requirements:
- Consistent environment for multiple programming languages and frameworks
- git-based
- Container Runtime availability
- Lightweight, ideally independent of local machine
- fast access, ideally no setup necessary
- Easy to share (and present)


- 12-factor X Dev/Prod Parity 
    - https://12factor.net/dev-prod-parity
    - idea to keep environments between dev, test and prod as consistent as possible
    - the tool gap
- Dev/Dev parity
    - make development environments as identical as possible
    - consistency in versions of Java, Maven, Gradle, Docker etc.
    - fast onboarding
    - (not so relevant in a proper CICD environment setup)

More Why? Scenarios

- Trying out things
- Trainings 
- Tutorials
- Multiple different projects and settings


Github / Codespaces
- github.dev
- access to codespaces

Links:
- https://docs.github.com/en/billing/managing-billing-for-github-codespaces/viewing-your-github-codespaces-usage
- https://github.com/settings/billing


Devcontainer
- devcontainer.json
- https://github.com/microsoft/vscode-dev-containers/blob/main/containers/codespaces-linux/.devcontainer/Dockerfile
- https://github.com/microsoft/vscode-remote-try-java/tree/main/.devcontainer


Gitpod
- https://www.gitpod.io/
- https://gitpod.io/billing
- https://www.gitpod.io/docs/configure/workspaces/workspace-image


devpod.sh
- https://devpod.sh/
- https://devpod.sh/docs/what-is-devpod
- https://github.com/loft-sh/devpod/tree/main/.devcontainer


Samples:
- https://github.com/open-telemetry/opentelemetry-demo
- https://opentelemetry.io/docs/demo/docker-deployment/