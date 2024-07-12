# `slingr` - Bash Script

This script allows you to 

## Requirements

- Bash 4 or higher
- `jq`

## Installation

Clone this repository and copy the executable file to some directory of
your `$PATH`.

```bash
git clone https://github.com/espinosajuanma/slingr-bash.git
cp ./slingr-bash/slingr /dest/path
```

### Symbolic Link

Or you can use a symbolic link to have multiple copies of the script and
be able to have different configurations for each one. If you want to
handle several apps and environments this is the way to go.

```
ln -s $PWD/slingr-bash/slingr $HOME/scripts/slingr-app
```

## Usage

- `slingr` - Prints current environment
  - Same as `slingr current`

## Configurations

- `slingr app [app]` - Configures app name
- `slingr env [env]` - Configures environment
  - Only accepts `dev`, `staging` or `prod`
- `slingr email [email]` - Configures login email

## Data

- `slingr query [entity] --field-name [field-value]`
  - Get
- `slingr record [entity] [record-id]`

## Developers

- `slingr console [path]` - 

### Tab completion

Use `complete -C slingr slingr` or put it in your `.bashrc` file to allows
tab completion.

## External credits

- The bash boilerplate was made by [rwxrob](https://github.com/rwxrob/template-bash-command)
