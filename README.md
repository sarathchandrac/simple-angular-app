# Simple Angular App
Simple Boiler plate for Angular App

# Angular Notes:
## Installation:
1. Install node
    - [Download](https://nodejs.org/en/download/) Node.js Installer 
	
	
	- Verify Installation after installation is complete:

```
	node -v
```
	- Update Node with latest version:
```
	npm install -g npm
```

2. The Angular CLI
```
    npm install -g @angular/cli
```
3. Create a New Project:
```
    ng new "my-new-angular-app"
    # options for enable routing : y
    cd "my-new-angular-app"
```
Note: if errors in installing all packages do `npm i` to install all dev packages locally
4. Run Angular locally at http://localhost:4200/:
```
    ng serve
```

## Add new pages:
```
ng generate component my-new-component
ng g component my-new-component #alias-name

```

