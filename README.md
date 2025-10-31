# Description

This repository contains the tests carried out to optimize the initial instruction prompt provided to gpt-realtime.  
The final goal is to obtain a valid prompt for the following use case:  
gpt-realtime must correctly and appropriately answer spoken questions related to the loaded tactile drawing.

# Organization

Each directory corresponds to a single interaction with gpt-realtime.  
The directories are ordered to create a consistent historical record.

Each directory contains the following information:

- Directory **"prompts"**:  
  contains:  
  - File **"initial_prompt.md"**: the prompt used in the test.  
  - File **"final_prompt.md"**: the prompt obtained after the modifications.  
  - File **"diff_prompt.md"**: the differences between the initial and final prompts.

- File **"interaction.jsonl"**:  
  contiene i messaggi scambiati tra utente e LLM durante l'interazione.

- File **.camio** (rename the extension to .zip to view its contents):  
  contains the drawing information that is passed to the LLM at the beginning of the interaction through dedicated messages.

- File **"problems_and_solutions.md"**:  
  contains the description of the issues encountered during the test and the proposed solutions to address them.  
  Note: the proposed solutions are not verified in the same test, but in subsequent ones.