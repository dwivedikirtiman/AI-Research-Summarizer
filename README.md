# 🤖 Research Assistant - AI Summarizer Extension

## Overview
The **Research Assistant** is a powerful Chrome extension integrated with a Spring Boot backend that leverages the **Gemini API** to summarize selected text from websites. The extension also features a note-taking area where users can save key summaries for future reference.

## 🛠️ Features
- ✅ Summarizes selected text from any webpage using the **Gemini API**
- ✅ Easy-to-use Chrome extension interface
- ✅ Textarea to save important summaries for future reference
- ✅ Seamless integration with Spring Boot backend
- ✅ Clean and visually appealing UI for better user experience

## 📁 File Structure
```
├── Research-Assistant-EXT (Frontend - Chrome Extension)
│   ├── background.js
│   ├── manifest.json
│   ├── sidepanel.css
│   ├── sidepanel.html
│   └── sidepanel.js
│
├── research-assistant (Backend - Spring Boot Project)
│   ├── src
│   │   ├── main
│   │   │   ├── java/com.research.assistant
│   │   │   │   ├── GeminiResponse.java
│   │   │   │   ├── ResearchAssistantApplication.java
│   │   │   │   ├── ResearchController.java
│   │   │   │   ├── ResearchRequest.java
│   │   │   │   ├── ResearchService.java
│   │   │   │   └── WebClientConfig.java
│   │   ├── resources
│   │   │   ├── static
│   │   │   ├── templates
│   │   │   └── application.properties
│   │
│   ├── .gitignore
│   ├── HELP.md
│   ├── mvnw
│   ├── mvnw.cmd
│   └── pom.xml
```

## 🔧 Setup Instructions
### Step 1: Clone the Repository
```bash

git clone https://github.com/dwivedikirtiman/AI-Research-Summarizer.git

```

Locate the project folder

```
cd research-assistant

```

### Step 2: Backend Setup (Spring Boot)
1. Open the **`research-assistant`** folder in IntelliJ IDEA.
2. Make sure your `application.properties` is properly configured:
```properties
server.port=8080
gemini.api.key=YOUR_GEMINI_API_KEY
```
3. Run the `ResearchAssistantApplication` class to start the backend server.

### Step 3: Frontend Setup (Chrome Extension)
1. Open the **`Research-Assistant-EXT`** folder in Visual Studio Code (VS Code).
2. Open Chrome and go to `chrome://extensions/`
3. Enable **Developer mode** (toggle on the top right).
4. Click **"Load unpacked"** and select the `Research-Assistant-EXT` folder.

### Step 4: Testing the Project
1. Select any text on a webpage.
2. Click on the extension icon in Chrome.
3. The summarized content should appear in the extension's panel.
4. Use the provided textarea to save key points.

## 🔍 Usage Guide
- Highlight text from any webpage.
- Click the **Research Assistant** extension icon.
- View the summarized content instantly.
- Save your summarized text for later reference in the provided text area.

## ✨ Future Improvements (Optional)
- 📊 Add user authentication to manage saved notes securely.
- 🔮 Improve UI with better visual design.
- 🔄 Implement multi-language support for broader accessibility.

## ⚙️ Contribution
Contributions are welcome! Feel free to raise issues or submit pull requests to improve the project.

## ℹ️ License
This project is licensed under the [MIT License](LICENSE).

## 👨‍💻 Author
**[Your Name]**  
[GitHub Profile](https://github.com/your-profile)  
[Email](mailto:your-email@example.com)

Still pending the read me file will be updated soon...

