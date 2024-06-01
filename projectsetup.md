### Steps
1. Created virtual env 
     * python3 -m venv ~/.venvs/pragent (user python3 to create env with python version 3.11 (non default))
     * source ~/.venvs/pragent/bin/activate

2. Set pathpath e.g export PYTHONPATH=. [Current directory from project root folder]
3. Created auth (bearer) token from bitbucket account
4. Edit the settings/configuration.toml file like git provider, model and other params
5. create .secrets.toml file by copying secrets_templat.toml
6. Run the server - python pr_agent/servers/bitbucket_server_webhook.py
7. Setup webhook in bitbucket - http://host.docker.internal:3000 (To call host machine url inside from container) 