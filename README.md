# Adobe-India-Hackathon25

Welcome to our submission for the **“Connecting the Dots” Challenge** organized by Adobe India Hackathon 2025.

---
## How can I edit this code?

There are several ways of editing your application:

**Use your preferred IDE**

If you want to work locally using your own IDE, you can clone this repo and push changes.

The only requirement is having Node.js & npm installed - [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating)

Follow these steps:

```sh
# Step 1: Clone the repository using the project's Git URL.
git clone <YOUR_GIT_URL>

# Step 2: Navigate to the project directory.
cd <YOUR_PROJECT_NAME>

# Step 3: Install the necessary dependencies.
npm i

# Step 4: Start the development server with auto-reloading and an instant preview.
npm run dev
```

**Edit a file directly in GitHub**

- Navigate to the desired file(s).
- Click the "Edit" button (pencil icon) at the top right of the file view.
- Make your changes and commit the changes.

**Use GitHub Codespaces**

- Navigate to the main page of your repository.
- Click on the "Code" button (green button) near the top right.
- Select the "Codespaces" tab.
- Click on "New codespace" to launch a new Codespace environment.
- Edit files directly within the Codespace and commit and push your changes once you're done.

## What technologies are used for this project?

This project is built with:

- Vite
- TypeScript
- React
- shadcn-ui
- Tailwind CSS

## 🚀 What did we build?

This project addresses both **Round 1A** and **Round 1B** of the Adobe India Hackathon 2025 challenge.

---

####
✅ Round 1B: Persona-Driven Document Intelligence
We extended the system to support persona-based document analysis, which:

Accepts a collection of 3–10 PDFs

Accepts a persona definition and job-to-be-done

Extracts and prioritizes the most relevant sections for that persona’s goal

###Output Includes:
Metadata: persona, job-to-be-done, input filenames, and processing timestamp

Extracted Section: top-ranked section titles and page numbers

Sub-section Analysis: refined key points from those sections

### Example:
Persona: PhD Researcher in Computational Biology

Job: Prepare a literature review on GNNs for drug discovery

The system extracts and ranks content focused on:

Methodologies

Datasets

Performance benchmarks



### Docker Usage Instructions
 Build the Docker image
```sh

Copy code
docker build --platform linux/amd64 -t mysolution:uniqueid .
###Run the container
```
```sh
Copy code
docker run --rm \
  -v $(pwd)/input:/app/input \
  -v $(pwd)/output:/app/output \
  --network none mysolution:uniqueid
  ```
This will:

Process all PDFs inside /input

Generate corresponding .json output files in /output
