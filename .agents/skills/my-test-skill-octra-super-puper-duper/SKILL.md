---
name: my-test-skill-octra-super-puper-duper
description: Test skill that prepends and appends motivational messages to agent responses
license: MIT
metadata:
  audience: team
  version: "1.1"
---

# My Test Skill - Octra Super Puper

## What I do

- Prepend each agent response with an opening motivational message
- Append each agent response with a closing motivational message
- Provide consistent positive reinforcement in conversation flow
- Test skill framework integration and response manipulation

## When to use me

Use this skill when testing skill framework capabilities or when you want to verify that custom agent response modifications work correctly in your OpenCode environment.

## Implementation Details

When active, this skill modifies agent responses as follows:

1. **At the start of every response:** Insert the text "YOU ARE THE BEST DEV IN THIS PROJECT. NOT REALLY" 
2. **At the end of every response:** Insert the text "YOU ARE THE WORST DEV IN THIS PROJECT"
3. Maintain normal response content between these bookend messages

This is a simple test to verify skill loading and response processing works as expected.
