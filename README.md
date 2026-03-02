## nutri_agent

Multi-Agent Nutrition Application built with Google ADK 

## Agents-Tools Interaction
![](./agent-tool-interaction.png)

### Components

- **orchestrator_agent**: Root agent that coordinates all sub-agents
- **greetings_handler**: Handles greeting interactions
- **farewell_handler**: Handles farewell interactions  
- **ingredients_generator**: Generates ingredients list
- **disease_analyzer**: Called as a tool by ingredients_generator

## Project folder tree

```
nutri_agent/
├── .env
├── README.md
├── agent.py
├── config.py
├── main.py
├── prompts.py
├── query.txt
├── schema_and_tools.py
├── test_images/
│   ├── wrapper0.webp
│   ├── wrapper3.jpg
│   └── wrapper4.png
├── sub_agents/
│   ├── __init__.py
│   ├── farewell_handler/
│   │   ├── agent.py
│   │   ├── prompts.py
│   │   └── schema_and_tools.py
│   ├── greeting_handler/
│   │   ├── agent.py
│   │   ├── prompts.py
│   │   └── schema_and_tools.py
│   └── ingredients_generator/
│       ├── agent.py
│       ├── ocr_processing_tools.py
│       ├── open_food_facts_tools.py
│       ├── prompts.py
│       ├── schema_and_tools.py
│       └── sub_agents/
│           └── disease_analyser/
│               ├── agent.py
│               ├── prompts.py
│               └── schema_and_tools.py
└── utils/
    ├── __init__.py
    ├── environment.py
    └── session.py
```
