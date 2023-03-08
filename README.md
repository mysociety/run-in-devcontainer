# Run command in dev-container

Version: 1.0.0

Run a series of commands inside the default devcontainer

## Usage

```yaml

- uses: mysociety/run-in-devcontainer@eaee6c314fb23ab625906c6b2d1fff7fe1b77041 # v1.0.0
  id: example-step 
  with:
    run: '' 
    shell: 'bash --noprofile --norc -eo pipefail'  # default
    app: 'app'  # default

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

docker-compose app to run command in

Default: app

