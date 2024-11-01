# Run command in dev-container

Version: 1.1.1

Run a series of commands inside the default devcontainer

## Usage

```yaml

- uses: mysociety/run-in-devcontainer@v1.1.1 # Replace with commit hash for safety
  id: example-step 
  with:
    run: '' 
    shell: 'bash --noprofile --norc -eo pipefail'  # default
    app: 'app'  # default
    dockerfile: 'Dockerfile.dev'  # default

```

## Inputs

### run

Required.

Commands to run inside context

### shell

shell to run command on inside docker

Default: bash --noprofile --norc -eo pipefail

### app

Required.

docker compose app to run command in

Default: app

### dockerfile

Dockerfile to build

Default: Dockerfile.dev

