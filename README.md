# 🤖 Research Assistant - AI Summarizer Extension

## Overview
The **Research Assistant** is a powerful Chrome extension integrated with a Spring Boot backend that leverages the **Gemini API** to summarize selected text from websites. The extension also features a note-taking area where users can save key summaries for future reference.

## 🛠️ Features
- ✅ Summarizes selected text from any webpage using the **Gemini API**
- ✅ Easy-to-use Chrome extension interface
- ✅ Textarea to save important summaries for future reference
- ✅ Seamless integration with Spring Boot backend
- ✅ Clean and very simple UI for better user experience

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

1. Open the **`research-assistant`** folder in IntelliJ IDEA with all the required dependencies, it's better to choose ```pom.xml``` file for opeining so that the IDE will automatically install all the important dependencties and the resources required for your application in order to run properly.

2. Make sure your `application.properties` is properly configured:
```properties

spring.application.name=research-assistant
gemini.api.url=https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=
gemini.api.key=${GEMINI_KEY}

```
**IMPORTANT NOTE** 

-  Make sure to edit the configuration setting of your IDE and adding your actual API_KEY under the environment variable place like this :

  ![image](https://github.com/user-attachments/assets/5aa36642-3c3a-418f-a054-16ba0a0e600e)

After adding your API_KEY click on "Apply" and then click on "OK" Button.

3. Look for all the required java file in the backend application and if there is no error then you're good to go further.
  
4. Run the `ResearchAssistantApplication` class to start the backend server.

5. Now, that the server is running fine and all the file is now set-up properly, you need to test your API in POSTMAN that whether it is giving the proper response by hitting the provided URL/URI, for that open your POSTMAN Application and create a new collection with any prefered name and then import the CURL which you've copied from GEMINI_API_KEY Page and also create one API_KEY(put it very private to you ) and then paste the URL in the import section and the page will look something like this:

![image](https://github.com/user-attachments/assets/0915ec9c-8dcc-4e0d-bed2-d3d6c0dd5967)

The Body part should be looking like this:

![image](https://github.com/user-attachments/assets/81814134-5ba0-4ffe-9ab5-1593edb5128a)

And finally if your backend application is running i.e. server is starting without any error then test/send the POST Request in POSTMAN and this should give some response to your given texts as follows:

![image](https://github.com/user-attachments/assets/c64d1506-9c1e-4bee-bcfa-004e97385089)



### Step 3: Frontend Setup (Chrome Extension)
1. Open the **`Research-Assistant-EXT`** folder in Visual Studio Code (VS Code).
2. Open Chrome and go to `chrome://extensions/`
3. Enable **Developer mode** (toggle on the top right).
4. Click **"Load unpacked"** and select the `Research-Assistant-EXT` folder.

### Step 4: Testing the Project
1. Select any text on a webpage.
2. Click on the extension icon in Chrome.
3. The summarized content should appear in the extension's panel, better to pin the extenstion for future use.
4. Use the provided textarea to save key points.

## Screenshots/Snapshots of the final output 

- Visit any document or any web page and select the texts which you want to summarize and the extension will summarize that for you like :

  ![image](https://github.com/user-attachments/assets/1186198f-f90a-4222-902a-69ffa226bb6e)

- If you want to save some result data then, the extension has a text area where you can put your data and this will save that preferred result for your future use like :

  ![image](https://github.com/user-attachments/assets/05cd6e9f-3b5a-4a97-8a6b-6d9733f1afa6)

- And finally, if you visit the extension after some time or close the extension and then open again the saved data will be there as this data is stored locally :

  ![image](https://github.com/user-attachments/assets/4e1e8369-cc49-42ff-b1af-3a7e7ed5751d)


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

**[Kirtiman Dwivedi]**

GitHub: https://github.com/dwivedikirtiman

Linkedin: https://www.linkedin.com/in/kirtiman-dwivedi/

Email: [dwivedikirtiman000@gmail.com]

Let’s connect—I’d love to hear your feedback! 🚀

