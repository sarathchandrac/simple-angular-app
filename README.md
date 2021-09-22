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
# ng g component my-new-component #alias-name
ng g component page-one

```
## Load page-one component in the home page
- add path to routes in `app-routing.module.ts`
~~~
import { PageOneComponent } from './page-one/page-one.component';
-----
const routes: Routes = [
  { path: 'page-one', component: PageOneComponent },
];
~~~
- add navigational link to `app.component.html`
~~~
<h1>Angular Router App</h1>
<!-- This nav gives you links to click, which tells the router which route to use (defined in the routes constant in  AppRoutingModule) -->
<nav>
  <ul>
    <li><a routerLink="/page-one" routerLinkActive="active">Page One</a></li>
  </ul>
</nav>
<!-- The routed views render in the <router-outlet>-->
<router-outlet></router-outlet>
~~~
- 


