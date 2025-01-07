# AI Agent Personalities

This repository contains a collection of personality configurations for AI agents designed to enhance interactions by providing diverse and customizable behaviors.

## Table of Contents

- [Introduction](#introduction)
- [Usage](#usage)
- [Personality Structure](#personality-structure)
- [Contributing](#contributing)
- [License](#license)

## Introduction

AI agents can be tailored to exhibit specific personalities, making interactions more engaging and contextually appropriate. This repository offers a variety of predefined personalities that can be easily integrated into your AI systems.

## Usage

1. **Select a Personality**: Browse the `personalities` directory to choose a suitable personality profile.
2. **Load the Configuration**: Integrate the selected personality into your AI agent by loading its configuration file.
3. **Apply the Personality**: Configure your AI agent to adopt the traits and behaviors defined in the chosen profile.

For example, in Python:

```python
import json

with open('personalities/godcat', 'r') as file:
    personality = json.load(file)

ai_agent.apply_personality(personality)
```

## Personality Structure

Each personality is defined in a JSON file with the following fields:

- `name`: The name of the personality.
- `description`: A brief overview of the personality's characteristics.
- `traits`: Specific attributes that define the personality's behavior.
- `dialogue_style`: Guidelines for the agent's communication style.
- `knowledge_base`: Domain-specific knowledge pertinent to the personality.

Example structure:

```json
{
  "name": "Empathetic Listener",
  "description": "An AI agent that provides empathetic and supportive responses.",
  "traits": {
    "empathy": 9,
    "patience": 8,
    "formality": 5
  },
  "dialogue_style": {
    "greeting": "Hello! I'm here to listen and support you.",
    "farewell": "Take care! Remember, I'm always here if you need to talk."
  },
  "knowledge_base": [
    "active listening techniques",
    "emotional support strategies"
  ]
}
```

## Contributing

Contributions are welcome! If you'd like to add a new personality or improve existing ones:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/new-personality`.
3. Commit your changes: `git commit -m 'Add new personality'`.
4. Push to the branch: `git push origin feature/new-personality`.
5. Submit a pull request.

Please ensure your contributions adhere to the existing format and include a comprehensive description.

## License

This project is licensed under the [MIT License](LICENSE).
