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
----

Increase Hermes Memory (Config)
Open Hermes config:

nano ~/.hermes/config.yaml

Find this section:

memory:
  memory_enabled: true
  user_profile_enabled: true
  memory_char_limit: 2200
  user_char_limit: 1375

Replace it with a larger memory configuration:

memory:
  memory_enabled: true
  user_profile_enabled: true
  memory_char_limit: 50000
  user_char_limit: 20000
  provider: holographic
