# Install Hermes
curl -fsSL https://raw.githubusercontent.com/NousResearch/hermes-agent/main/scripts/install.sh | bash

# Update Hermes
hermes update

# Change Model
hermes model

# Set API Key
hermes config set GOOGLE_API_KEY TU_API_KEY

# Run Hermes
hermes

# Edit Config (increase memory)
nano ~/.hermes/config.yaml

Nano save commands:
CTRL + O
ENTER
CTRL + X
