Walkthrough:

Title
About me
XXX

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
- https://github.com/codespaces

#Spring Boot


```bash
curl https://start.spring.io
curl https://start.spring.io/starter.zip -d type=maven-project -d dependencies=web,actuator -o demo.zip 
curl https://start.spring.io/starter.zip -d type=maven-project -d dependencies=web,actuator,devtools -d name=other -o other.zip
```

cmd+shift+p:
Java: Import Java Projects
Workspace: Remove Folder



Check for Java projects lower left and add them

https://www.baeldung.com/spring-rest-openapi-documentation

Look into devcontainer.json
and settings.json


Host Info:
uname -a
lscpu
cat /proc/meminfo


Links:
- https://docs.github.com/en/billing/managing-billing-for-github-codespaces/viewing-your-github-codespaces-usage
- https://github.com/settings/billing


Devcontainer
- devcontainer.json
- https://hub.docker.com/_/microsoft-devcontainers-universal
- https://github.com/microsoft/vscode-dev-containers/blob/main/containers/codespaces-linux/.devcontainer/Dockerfile
- https://github.com/microsoft/vscode-remote-try-java/tree/main/.devcontainer


Gitpod
- https://www.gitpod.io/
- https://gitpod.io/billing

- brave://extensions/
  
- https://www.gitpod.io/docs/introduction/languages/java

  
- https://www.gitpod.io/docs/configure/workspaces/workspace-image
- https://github.com/gitpod-io/workspace-images
- https://github.com/docker-library/buildpack-deps


devpod.sh
- https://devpod.sh/
- https://devpod.sh/docs/what-is-devpod
- https://github.com/loft-sh/devpod/tree/main/.devcontainer


Samples:
- https://github.com/open-telemetry/opentelemetry-demo
- https://opentelemetry.io/docs/demo/docker-deployment/


Container stuff:

docker 

sudo add-apt-repository ppa:cncf-buildpacks/pack-cli
sudo apt-get update
sudo apt-get install pack-cli



Shell stuff:

zsh/fzf:
git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
~/.fzf/install

brew install fzf
/opt/homebrew/opt/fzf/install

bindkey "^[[A" fzf-history-widget
bindkey "${terminfo[kcuu1]}" fzf-history-widget

without omz
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions
source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh

with omz
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
plugins=( 
    # other plugins...
    zsh-autosuggestions
)

omz theme list
omz theme
omz theme use agnoster
omz set agnoster
omz theme set agnoster

https://github.com/ohmyzsh/ohmyzsh/wiki


old:
docker init does not work
add to devcontainer.json
