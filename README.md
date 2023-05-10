# GrowthBook CLI

A CLI tool for helping developers work with the GrowthBook open-source platform for feature flags and A/B tests. 

See the [official GrowthBook CLI](https://docs.growthbook.io/tools/cli) documentation for more information.

# Commands

<!-- commands -->
* [`growthbook auth`](#growthbook-auth)
* [`growthbook auth login`](#growthbook-auth-login)
* [`growthbook auth logout`](#growthbook-auth-logout)
* [`growthbook features`](#growthbook-features)
* [`growthbook features generate-types`](#growthbook-features-generate-types)
* [`growthbook features toggle FEATUREKEY`](#growthbook-features-toggle-featurekey)
* [`growthbook help [COMMANDS]`](#growthbook-help-commands)

## `growthbook auth`

```
USAGE
  $ growthbook auth
```



## `growthbook auth login`

Configure your API key with the GrowthBook SDK with your project

```
USAGE
  $ growthbook auth login

DESCRIPTION
  Configure your API key with the GrowthBook SDK with your project
```

## `growthbook auth logout`

Removes GrowthBook API key configurations

```
USAGE
  $ growthbook auth logout [-p <value>]

FLAGS
  -p, --profile=<value>  Optional profile (for projects that use multiple GrowthBook instances or organizations)
                         (default: all profiles)

DESCRIPTION
  Removes GrowthBook API key configurations
```

## `growthbook features`

```
USAGE
  $ growthbook features
```



## `growthbook features generate-types`

Generate TypeScript types for all your features

```
USAGE
  $ growthbook features generate-types [-u <value>] [-p <value>] [-o <value>]

FLAGS
  -o, --output=<value>      Output path for the app-features.ts file. All directories in this path should exist. If not
                            provided, the directory ./growthbook-types will be created in the current working directory.
  -p, --profile=<value>     Optional profile (for projects that use multiple GrowthBook instances) default: default)
  -u, --apiBaseUrl=<value>  Your GrowthBook instance base URL (e.g. http://localhost:3100, default:
                            https://api.growthbook.io)

DESCRIPTION
  Generate TypeScript types for all your features
```

## `growthbook features toggle FEATUREKEY`

Toggle a feature on or off for a specific environment

```
USAGE
  $ growthbook features toggle FEATUREKEY -e <value> -n true|false|on|off|1|0 [-u <value>] [-p <value>] [-r <value>]

ARGUMENTS
  FEATUREKEY  Feature key to toggle

FLAGS
  -e, --environment=<value>  (required) Environment that you would like to toggle
  -n, --enabled=<option>     (required) Enabled state of the feature
                             <options: true|false|on|off|1|0>
  -p, --profile=<value>      Optional profile (for projects that use multiple GrowthBook instances) default: default)
  -r, --reason=<value>       The reason for toggling it on
  -u, --apiBaseUrl=<value>   Your GrowthBook instance base URL (e.g. http://localhost:3100, default:
                             https://api.growthbook.io)

DESCRIPTION
  Toggle a feature on or off for a specific environment

EXAMPLES
  $ growthbook features toggle
```

## `growthbook help [COMMANDS]`

Display help for growthbook.

```
USAGE
  $ growthbook help [COMMANDS] [-n]

ARGUMENTS
  COMMANDS  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for growthbook.
```


<!-- commandsstop -->
