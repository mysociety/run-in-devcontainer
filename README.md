# Run command in dev-container

Version: 1.0.1

Run a series of commands inside the default devcontainer

## Usage

```yaml

- uses: mysociety/run-in-devcontainer@2200446d40095780e7271c0ea73497ed2bd68b99 # v1.0.1
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

