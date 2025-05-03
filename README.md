# Summarize & Visualize

A React application that allows users to upload text or paste content, generates a summary using AI, and creates visual representations based on the summary text.

## Features

- Text input via direct pasting or file upload
- AI-powered text summarization using Gemini API
- Image generation based on summary using Hugging Face Stability AI model
- Ability to edit summaries and regenerate images
- Loading indicators during API processing
- Responsive design with TailwindCSS

## Tech Stack

- **Frontend**: React (Vite)
- **Styling**: TailwindCSS
- **APIs**:
  - Gemini API for text summarization
  - Hugging Face Stability AI for image generation

## Getting Started

### Prerequisites

- Node.js and npm installed on your machine
- API keys for:
  - Gemini API
  - Hugging Face

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/summarize-visualize.git
   cd summarize-visualize
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory and add your API keys:
   ```
   VITE_GEMINI_API_KEY=your_gemini_api_key
   VITE_HUGGINGFACE_API_KEY=your_huggingface_api_key
   ```

4. Update the API keys in App.jsx:
   - Replace `YOUR_GEMINI_API_KEY` with `import.meta.env.VITE_GEMINI_API_KEY`
   - Replace `YOUR_HUGGINGFACE_API_KEY` with `import.meta.env.VITE_HUGGINGFACE_API_KEY`

5. Start the development server:
   ```bash
   npm run dev
   ```

6. Open your browser and navigate to `http://localhost:5173`

## Deployment

This project can be deployed to various platforms like Vercel or Netlify:

### Deploying to Vercel

1. Install Vercel CLI:
   ```bash
   npm install -g vercel
   ```

2. Run deployment command:
   ```bash
   vercel
   ```

3. Follow the prompts and add your environment variables for API keys

### Deploying to Netlify

1. Build the project:
   ```bash
   npm run build
   ```

2. Upload the build directory to Netlify or connect your GitHub repository

3. Set the environment variables in the Netlify dashboard

## Usage

1. Paste text or upload a text file in the input area
2. Click "Generate Summary" to create a summary using AI
3. The application will automatically generate an image based on the summary
4. Edit the summary if needed and click "Regenerate Image" to create a new visualization

## Future Enhancements

- Multiple image generation for each summary
- Save history of summaries and visualizations
- Additional styling options for images
- Support for more file formats
- Export functionality for generated content

## License

This project is licensed under the MIT License - see the LICENSE file for details.
