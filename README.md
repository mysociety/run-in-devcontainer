# Run command in dev-container

Version: 1.0.2

Run a series of commands inside the default devcontainer

## Usage

```yaml

- uses: mysociety/run-in-devcontainer@dc063e6c8ae7a2b4162c1c10a7a99bcaf2df8b1e # v1.0.2
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

docker compose app to run command in

Default: app

