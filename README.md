# deploy-bot-action
This action allows [Botonic](https://botonic.io/) users Build &amp; [Deploy to Hubtype](https://botonic.io/docs/deployment/hubtype) a bot using Github actions


# Usage

See [action.yml](action.yml)

```yaml
env:
    BOTONIC_CLIENT_ID: xxx
    BOTONIC_URL: yyy
    # TODO setup the rest of Hubtype env vars needed

steps:
    uses: actions/checkout@v2 # checkout the code of your bot

    uses: hubtype/deploy-bot-action@v1
    with:
        BOT_SRC_DIR: your_bot_src_dir
        BOT_NAME: your_bot_name
        USERNAME: hubtype_user_to_deploy_bot
        PASSWORD: hubtype_pass_to_deploy_bot
```

# License
The scripts and documentation in this project are released under the [MIT License](LICENSE)

