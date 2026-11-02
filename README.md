# Escalate-or-Answer
How Should an Agentic RAG Assistant Hand Back a Decision That Depends on the User?
CS 567, Fall 2026, Colorado State University
Group: CS567_Coen_Cam_Context_Not_Found
Members: Coen Petto (coenp@colostate.edu), Cameron Suess (camsuess@colostate.edu)

### Checkpoint Videos
* https://youtu.be/JR6AXOra5UM (Checkpoint 1)
* https://youtu.be/JJKzbRxvmpI (Checkpoint 2)
* https://youtu.be/wayJk7t3mRk (Checkpoint 3)

### Paper Links
* https://www.overleaf.com/read/jrrsqpgrjsmw#c44e63

### Prototype pipeline (`system/`)
A local, reproducible version of the study pipeline lives in [`system/`](system/README.md): SNA snapshot → chunks → FictionalQA-style blind/informed filter → embedding index → fork check → frozen v4 task records → playground with the three escalation forms. It runs on Ollama (Windows/CUDA or macOS/Metal). Quick start: install Ollama, then `cd system && pip install -r requirements.txt && python -m escalate setup && python -m escalate serve`.
