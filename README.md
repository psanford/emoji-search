# Emoji Search

This is a SPA for searching a large export of emoji (say from Slack). It loads emoji data from a CSV file and provides real-time search functionality.

## CSV Format

The application expects the CSV file to have the following format:

```
name,url
emoji_name,https://example.com/emoji.png
alias_name,alias:original_emoji_name
```

- The first line should be the header: `name,url`
- Each subsequent line represents an emoji or an alias
- For regular emojis: `emoji_name,image_url`
- For aliases: `alias_name,alias:original_emoji_name`


## Generating the CSV File from Slack

You can generate a CSV from a slack workspace using the [slack-emoji-fetch](https://github.com/psanford/slack-emoji-fetch) tool.
