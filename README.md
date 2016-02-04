# Slack Emoji Search

A commandline utility to search across Slack for messages that were reacted to with a specific emoji.

## Installation

The simplest way to install this package is to use [pip](https://pip.pypa.io/en/stable/installing/) to install the package from the [Python Package Index](https://pypi.python.org/pypi/slack-emoji-search):

    $ pip install slack-emoji-search

## Usage

You will need a Slack API key. You can get this from the [Slack website](https://api.slack.com/web). The script expects the token to be provided via the `--api-token=<MY-API-TOKEN>` command line option.

To query for messages reacted to with the :evergreen_tree: emoji between Nov 2, 2015 and Oct 31, 2015 and write the output to a file called evergreen.txt in the current directory, run:

    emoji_search --api-token <MY-API-TOKEN> \
                 --emoji evergreen_tree \
                 --startdate 10-31-2015 \
                 --enddate 11-02-2015 \
                 --outfile evergreen.txt

All flags are optional except for --emoji. If no destination file is provided, results will be written to the terminal.

## Public Domain

18F's work on this project is in the worldwide [public domain](LICENSE.md).

> This project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/).
>
> All contributions to this project will be released under the CC0 dedication. By submitting a pull request, you are agreeing to comply with this waiver of copyright interest.
