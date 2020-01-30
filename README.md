# trello_cli

This CLI Trello API client helps you extract and manipulate objects using JSON.

## Installation

1. Install [jq](https://stedolan.github.io/jq/)

2. Log into Trello and obtain your API key and token at https://trello.com/app-key.

3. Set the following variables (i.e. in ~/.profile)

  ```
  export trello_cache_dir=
  export trello_key=
  export trello_token=
  ```

## Usage

* `clitrello boards`

* `clitrello cards 'boardid'`

  Read cards from board 'boardid'. 
  By environemnt var `$actions`, you can set more information to be printed.
  Default value: `$actions=commentCard`

  More information for actions can be found here: https://developers.trello.com/reference#section-nested-cards-as-url-params

* `clitrello search 'criteria'`

  Find all cards corresponding to the search criteria.

See `bin/clitrello` for the whole list of supported API methods.

