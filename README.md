# Description

This repository contains the tests carried out to optimize the initial instruction prompt provided to **gpt-realtime**.  
The final goal is to obtain a valid prompt for the following use case:  
gpt-realtime must correctly and appropriately answer spoken questions related to the loaded tactile drawing.

# Organization

Each directory corresponds to a single interaction with gpt-realtime.  
The directories are ordered to create a consistent historical record.

Each directory contains the following information:

- Directory **"prompts"**:
  - File **"initial_prompt.txt"**: the prompt used in the test.
  - File **"final_prompt.txt"**: the prompt obtained after the modifications. Note: the final prompt is not verified in the same test, but in subsequent ones.

- File **"interaction.txt"**:  
  contains the messages exchanged between the user and the LLM during the interaction.

- File **.camio** (rename the extension to .zip to view its contents):  
  contains the drawing information that is passed to the LLM at the beginning of the interaction through dedicated messages.

- File **"problems.txt"**:  
  contains the description of the issues encountered during the test.