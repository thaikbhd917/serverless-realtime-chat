.

├── fetchMessages               <-- Source code for get messages from DB

├── onConnect                   <-- Source code onConnect

├── sendMessage                 <-- Source code sendMessage

└── template.yaml               <-- SAM template for Lambda Functions and DDB

└── static                      <-- Frontend single page
# Deploying on your account
AWS CLI commands
AWS CLI commands to package, deploy and describe outputs defined within the cloudformation stack:

sam build

sam deploy --guided

# Setting endpoint for front-end
using deployed apigateway endpoint in static/index.js

const websocket_endpoint = "wss://#.execute-api.ap-northeast-1.amazonaws.com/Prod"

const fetch_messages_endpoint = "https://#.execute-api.ap-northeast-1.amazonaws.com/Prod/prod"

# Demo
https://d139yel1pz2zrl.cloudfront.net/
