# NPL dotenv

A nplc package aims to bring the advantages from the [dotenv](https://github.com/bkeepers/dotenv) to npl runtime!

## Usage

Simply add a .env file and put your kv config into it like this:

.env file

```sh
# comment
KEY=VALUE
```

in npl

```lua
print(ENV[KEY]) -- VALUE
```

Important, do NOT put comment to the tail of a kv config, like this:

```sh
KEY=VALUE # comment
```

In this way, you will get

```lua
print(ENV[KEY]) -- VALUE # comment
```
