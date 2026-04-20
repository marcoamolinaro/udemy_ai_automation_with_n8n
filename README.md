How to run n8n on docker desktop
    - execute docker desktop
    - open a terminal window in docker and type the commands:
        docker volume create n8n_data (for the first time to create folder)
        docker run -it --rm --name n8n -p 5678:5678 -v n8n_data:/home/node/.n8n -e N8N_RESTRICT_FILE_ACCESS_TO=/home/node/ docker.n8n.io/n8nio/n8n



How to use ollama
    - Go to ollama website and download, when the downloand finish execute the .exe, and following the instruction
    - When finishes the installation open a PS window as administrator and input the following command 
        ollama run deepseek-r1:7b after download and install close the ps window
    - Open another PS window and type ollama serve, copy the url and past on a new windows 
	  browser it should show the "Ollama is running" message



How to get credentials to google sheets or google email
    - In the n8n page connector, click on docs and then click on google account 
    - On google console go to API Library and enable Google Sheets API ou Google Gmail API
    - Create a new project 
    - On the left panel menu go to conset OAuth and Get Start
    - Choose "Web application" on Application Type
    - Go to Autorized Redirect URI and past the n8n URL that appears on n8n connector panel
    - Click on Create
    - Go on Consent and add a test user (use the same email you are login on google console)
    - Click on the edit icon on OAuth, copy the Client ID and Secret ID and past them on the n8n connector panel
    - On n8n connector panel click on Google sign in
    - On google sign in choose the email, check all, continue, and ok
    - Go Back on n8n connector page and see if a success mensage appears 
    - Following the steps to integrate to finish
