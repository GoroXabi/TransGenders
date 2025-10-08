# Mandatory Components (25%)
## Minimal Technical Components
* Backend not mandatory, but it needs to be in PHP
* Database not mandatory
* Frontend should be in TypeScript
* Site should be a [Single page application](https://en.wikipedia.org/wiki/Single-page_application)
* There shouldn't be errors or warnings
* Site must be dockeriezd
* Third party libraries or tools can't solve any entire module by themselves
## Game
* Pong should be played against other players in the site
	* I don't get if it should be played in same browser or if it's always remote (See remote players module)
* Tournament system should be implemented
* User registration (for Tournaments)
* Matchmaking system (pretty vague from subject)
* Rules should be equal, even for AI
* Game should either follow frontend technical constraints or Frontend module constraints, or Graphics Module.
## Security
* Passwords should be hashed. Hashing algorithm must be strong (maybe sha256?)
* Site must be protected from SQL injections
* If there is backend, HTTPS should be used for all aspects
* Implement or not JWT (dunno what that is). If you make an API, it should be route protected.
* Any credential, API keys, env vars etc should all be local and ignored by Git
# Modules
## Mandatory
* 7 points needed for 100%
* 1 point for major module
* 0.5 points for minor module
## Bonus
* 5 points of score for each minor module
* 10 points of score for each major module
(125% can be achieved for example with 2 major and one minor extra modules)
# Web
## Framework Module (Major)
Use Fastify with Node.js for the backend instead of PHP
### Framework Frontend Module (Minor)
Use Tailwind CSS in addition to TypeScript for the frontend
### Database Module (Minor)
Use SQLite as DB
## Blockchain Module (Major)
Store the score of the tournament in a blockchain. Avalanche is the blockchain system and Solidity it's programming language
# User Management
## Standard user management (Major)
* Users can subscribe and login to the server securely
* Users can select a unique display name in tournaments
* Users can update info
* Avatar management
* Users can add friends and see their status
* User profiles display stats and match history
## Remote auth (Major)
Implement OAuth 2.0
# Gameplay
## Remote players (Major)
Players can play in separate computers against each other
## Multiple players (Major)
Implement the game for more than two players
## Add second game (Major)
It needs to have user history and matchmaking
### Game customization (Minor)
Offer customization to all game(s). Maps, skins, powerups, etc. Basic version should still be accessible.
## Chat (Major)
Live chat, with DMs, blocking, game invites, tournament notifications and accessing profiles
# AI-Algo
## AI Opponent (Major)
Incorporate an AI player into the game. The A* algorithm is not allowed
* For some fucking reason the AI can only update 1 time per second???
* AI needs to have logic
* AI needs to adapt to the user and different gameplay scenarios
* The AI should be able to win sometimes
### User and Game Stats Dashboards (Minor)
Implement friendly dashboards for stats
# Cybersecurity
## WAF/ModSecurity (Major)
* WAF (Web Application Firewall) and ModSecurity need to be implemented with strict security
* HashiCorp Vault needs to be implemented to store information like API keys, credentials and env variables.
### GDPR compliance and anonymous users (Minor)
GDPR compliance features which enable users to request anonymization of their personal data. Also systems that implement personal data management to the user should be impelemented.
* Implement account and info deletion
* Inform clearly what privacy rights the users have
## 2FA and JWT (Major)
Implement 2FA and JWT (JSON Web Tokens) as a secure method for authentication
User friendly setup process for 2FA needed.
# DevOps
## Infrastructure setup with ELK for Log Management (Major)
Implement ELK (Elasticsearch, Logstash, Kibana) for log managemnet.
### Monitoring system (Minor)
Implement Prometheus and Grafana to monitor metrics and health of servoce
## Backend as Microservices (Major)
Divide backend into smaller microservices, so if one fails, the rest of the site still works.
Communication between them should be RESTFful. 
# Graphics
## Implement 3D (Major)
Develop the Pong game using Babylon.js
# Accesibility
### Support multiple devices (Minor)
Site should be responsive and easily navigable with desktops, tablets, laptops and smartphones
### Extend browser compatibility (Minor)
Make it compatible with another browser (Chromium basically)
### Multiple languages support (Minor)
Minimum three languages support (English, Spanish and Euskara)
### Accesibility for Visually Impaired Users (Minor)
Support for screen readers and similar techs, alt text, options for adjusting text size and keyboard navigation of the site
### Server-Side Rendering (Minor)
Implement SSR (Don't exactly know what it means)
# Server-Side Pong
## Replace Pong with SSPong (Major)
Implement the game in server, and implement an API for communicating with it.
## Pong playable via CLI (Major)
Allow people to play in CLI with an API against other CLI users or even web users
