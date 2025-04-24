# HyperMath_OpportunAI
# HyperMath: AI-powered Math Chatbot

HyperMath is an innovative, AI-powered chatbot-style web application that enables users to input math-related prompts and receive detailed explanations and dynamic visualizations of the concepts. By combining cutting-edge AI models (Gemini for natural-language processing and CodeGen for generating code) with powerful visualization tools (Manim), HyperMath brings math learning to life in an engaging, interactive manner. The app even provides optional speech overlays to further enhance the learning experience.

## Key Features

- **Natural-Language Explanations**: Uses a fine-tuned Gemini model to generate clear, detailed explanations of math concepts in natural language.
- **Interactive Visualizations**: Generates dynamic video visualizations of math concepts using the CodeGen model to produce Manim code.
- **Real-time Video Creation**: The Manim code is executed to generate a high-quality video that illustrates the concept being explained.
- **Speech Integration** (Optional): Converts the explanation text to speech using gTTS, then overlays the voice onto the video using MoviePy to create an immersive learning experience.
- **User-Friendly Chat Interface**: A simple, clean chat-style frontend for easy interaction with the AI chatbot.

## How It Works

1. **User Input**: The user enters a math-related query into the chat interface (e.g., "Explain the Pythagorean theorem").
2. **AI Explanation**: The input is sent to a fine-tuned Gemini model that generates a detailed natural-language explanation of the math concept.
3. **Visualization Generation**: The explanation is passed to a fine-tuned CodeGen model, which generates Manim code to create a corresponding math visualization.
4. **Manim Code Execution**: The backend executes the Manim code to generate a video that visualizes the concept.
5. **Optional Speech Overlay**: The explanation is converted into speech using the Google Text-to-Speech (gTTS) library, and the voice is overlaid onto the video using MoviePy.
6. **Video Output**: The final video is returned to the user via the chat interface for viewing or download.

## Technologies Used

- **Flask**: Lightweight web framework for building the backend and handling API requests.
- **Gemini**: A fine-tuned AI model for natural-language explanation generation.
- **CodeGen**: A fine-tuned AI model for generating Manim code to create math visualizations.
- **Manim**: An animation engine for creating high-quality math visualizations.
- **gTTS**: Google Text-to-Speech API for converting the generated explanation to voice.
- **MoviePy**: A Python library used for video editing to overlay speech on the visualization.
- **Google Cloud Platform (GCP)**: Used for deploying AI models and handling cloud-based tasks.

## Installation & Setup

### Prerequisites

- Python 3.x
- Google Cloud account (for accessing the fine-tuned Gemini )
- Manim library installed locally for generating math visualizations
- Flask for backend development
- gTTS for speech generation
- MoviePy for video editing

### Steps to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/HyperMath.git
   cd HyperMath
