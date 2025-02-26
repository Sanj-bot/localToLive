# localToLive

- ### Problem Statement:
    - I often face problem when i build a website and i wanna share it to my friends but i have to use a cloud service to deploy my project

- ### Solution:
    - I used ngrok( a reverse proxy) to deploy my app over internet 
- ### Tech Stack:
    - html/css/js
    - ngrok cli (other similar tools: ```https://theboroer.github.io/localtunnel-www/```,```https://localhost.run/docs/```)

- ### Method:
    - install ngrok agent: ```curl -sSL https://ngrok-agent.s3.amazonaws.com/ngrok.asc \
  | sudo tee /etc/apt/trusted.gpg.d/ngrok.asc >/dev/null \
  && echo "deb https://ngrok-agent.s3.amazonaws.com buster main" \
  | sudo tee /etc/apt/sources.list.d/ngrok.list \
  && sudo apt update \
  && sudo apt install ngrok```
  - ngrok help :```ngrok help```
  - connect acc:```ngrok config add-authtoken <TOKEN>```
  - put app online: ```ngrok http http://localhost:xxxx```(an app is working on this url)
  - you can use your app with custom url and provide security too.

- ### Docs:
    - https://ngrok.com/docs/getting-started/



- ### Insights:
    - reverse proxy: server that acts as mediator b/w client and web-server
