# Getting Started

1. install `uv` if you haven't `brew install uv`
2. run `uv run llamactl serve deployment.yaml`
3. Visit http://localhost:4501/ui/research/



# Organization

- `deployment.yaml` contains the llama_deploy configuration, telling it where to find workflows, which workflows to install, and where the ui is
- `src` contains python workflow sources. The name of the deployment here is defined as `research`
- `ui` contains a next.js app that calls the local workflow server via api requests. See http://localhost:4501/docs for openAPI docs
