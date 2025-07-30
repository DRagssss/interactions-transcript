# interactions-transcript

This project is built on an improved version of [mahtoid's DiscordChatExporterPy library](https://github.com/mahtoid/DiscordChatExporterPy), ported to an extension of interactions.py, another Discord API wrapper, with extra features. You can find the [archived original by ItsRqtl](https://github.com/ItsRqtl/interactions-transcript).

WIP: This extension is currently work-in-progress, which means it might not function well  

## Installation

### Install from github

```bat
pip install git+https://github.com/DRagssss/interactions-transcript.git
```

### Build from source

```bat
git clone https://github.com/DRagssss/interactions-transcript.git
cd interactions-transcript
pip install .
```

## Usage

### Using the extension

```py
await GuildText.get_transcript(limit=...)
```

### Using the extension

```py
from interactions import Client
from interactions.ext.transcript import get_transcript
...
await get_transcript(GuildText, limit=...)
...
client.start()
```

Parameters of method `get_transcript`:

|Parameter|Type|Description|Default Value|
|---|---|---|---|
|channel|`interactions.GuildText`|The channel to get transcript from||
|limit|`int`|The limit of messages to get|`100`|
|pytz_timezone|`str`|The timezone to use|`"UTC"`|
|military_time|`bool`|Whether to use military time or not|`False`|
|fancy_time|`bool`|Whether to use fancy time or not (only with html mode)|`False`|
|mode|`str`|The mode to use for the transcript (html, json, csv, or plain)|`"html"`|

## Attributions

This project is an up-to-date fork of the [repository by ItsRqtl](https://github.com/ItsRqtl/interactions-transcript) which uses a modified version of the parser, cache, html, and css code from [mahtoid's DiscordChatExporterPy library](https://github.com/mahtoid/DiscordChatExporterPy).

## License

This project follows the original library and is licensed under the `GNU General Public License v3.0`. Check the [LICENSE](/LICENSE) for more information.
