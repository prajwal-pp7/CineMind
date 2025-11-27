# cinemind-backend

# CineMind – Visual Narrative Generator (Backend Demonstration)

*Course:* DES646: AI/ML for Designers

---

## Overview

CineMind is a *conceptual backend demonstration* for a visual narrative generator. It illustrates how a short story prompt can be transformed into cinematic frames using AI, following the pipeline shown in the Figma prototype.  

This repository is for *demonstration purposes only* and does not require running the Stable Diffusion API.

---

## Purpose

This repository demonstrates the intended backend workflow of CineMind. It shows how a one-line story prompt can be analyzed for emotional tone and key visual elements, expanded into cinematic AI prompts, and converted into visual frames. The focus is on illustrating the *conceptual pipeline* rather than producing actual images. 
The prototypes can be viewed on Figma: 
[CineMind Prototype 1] (https://www.figma.com/design/WhpN8N0DtObnrDLCAKqpxA/Untitled?node-id=63-2&p=f&t=0BsEfLQ6s4F6W9XU-0)
[CineMind Prototype 2] (https://www.figma.com/design/WhpN8N0DtObnrDLCAKqpxA/Untitled?node-id=46-2&p=f&t=0BsEfLQ6s4F6W9XU-0)
[CineMind Prototype 3] (https://www.figma.com/design/WhpN8N0DtObnrDLCAKqpxA/Untitled?node-id=24-68&t=0BsEfLQ6s4F6W9XU-0)

---

## Demonstrated Pipeline

1. *Input:* Accept a one-line story prompt.  
2. *Mock NLP analysis:* Extract emotional tone and visual context.  
3. *Cinematic prompt expansion:* Generate AI-ready prompts with cinematic framing.  
4. *Image generation (simulated):* Intended API calls to Stable Diffusion (optional).  
5. *Output:* 4–5 cinematic frames saved locally (or simulated).

---

## Features

- Simulated NLP tone and setting detection.
- Automatic expansion of a story into multiple cinematic prompts.
- Integration with the Stable Diffusion API for frame generation (optional).
- Outputs a small cinematic sequence to visualize the story.

---

## Requirements

- Python 3.8+
- requests library

Install dependencies via pip:

```bash
pip install requests

A Stable Diffusion API key (optional; replace YOUR_STABILITY_API_KEY in the script).
For submission purposes, the code can run as a mock pipeline without actual API calls if the key is left blank.



---

Usage

1. Clone this repository:



git clone https://github.com/<username>/CineMind.git
cd CineMind

2. Update your API key in the script (optional):



API_KEY = "YOUR_STABILITY_API_KEY"

3. Run the demo script:



python cinemind_backend_demo.py

4. The script will:



Analyze the story prompt.

Generate cinematic AI prompts.

Save 4–5 frames under cinemind_outputs/ (if API key is provided).


Example output directory structure:

cinemind_outputs/
├── frame_1.png
├── frame_2.png
├── frame_3.png
├── frame_4.png
├── frame_5.png


---

Example

Example story prompt:

"A lonely man rides the metro at dawn"

The script outputs:

Detected emotional tones (solitude, dawn light, etc.)

Detected settings (metro station, train interior, etc.)

4–5 cinematic prompts simulating AI input for frame generation.


Sample cinematic prompt:

A lonely man rides the metro at dawn. wide-angle shot, moody lighting, solitude, metro station, cinematic film grain.

> Note: Frames will only be generated if a valid API key is provided. For submission, viewing the printed prompts is sufficient.




---

Notes

This project is a demonstration of the intended backend workflow.

The focus is on showing the conceptual pipeline, not full deployment.

No installation or API execution is required to understand the workflow.
