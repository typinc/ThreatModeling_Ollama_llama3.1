# README

## Instructions
* Install Ollama
* In a console: ollama run llama3.1
* In your venv: pip install -r requirements.txt
* Run generate_repository_profile.py to test if the setup is working

## Informations
* If you have a GPU installed, the FAISS library will use the GPU for the workload. If no GPU is detected, the workload will use your CPU.
* The content of the _chain.stream_ methode can be modified 
  * EXAMPLE: 
```
   Tell me the following information about the code base I am providing you:
     - Purpose of the application
     - Web technologies used in the vtm application
     - Templating language used in the vtm application
     - Database used in the vtm application
     - Authentication mechanisms used in the vtm application
     - Authorization mechanisms used in the vtm application
    
    List libraries by their name, purpose, and version that are
    used in the vtm application for the following categories:
        - Security
        - Testing
        - Documentation
        - Build
        - Database
        - Authentication / Authorization
        - HTML Templating (ex: pug, handlebars)
        - CSS Frameworks (ex: bootstrap, tailwind)
        - widgets / UI components
```