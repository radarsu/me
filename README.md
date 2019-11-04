<p align="center">
    <a href="https://github.com/radarsu/me/" target="blank" alt="me"><img src="https://github.com/radarsu/me/blob/master/assets/logo.png?raw=true" alt="me logo" /></a><br/>
</p>

<p align="center">
	<strong>Personal version of <a href="https://github.com/sindresorhus/awesome" target="_blank" alt="awesome">Awesome</a>, best practices and setups.</strong>
</p>

<p align="center">
	The purpose of this repository is to share resources and setups interesting for TypeScript, Node.js and JavaScript full-stack developers.
</p>

## Description
Awesome repositories are usually targetted at certain things like - programming language, technology, books, etc. This one is composition of completely different stuff that's just personal, but might be useful for any full-stack developer interested in JavaScript, Node.js, Typescript and Angular - or simply working on same platform as I am (currently Windows).

## Content
- [Community](#community)
  - [Gitter](#gitter)
- [Performance](#performance)
  - [Loops](#loops)
  - [DOM](#dom)
- [Practices](#practices)
  - [Comments](#comments)
  - [Naming](#naming)
  - [Other Practices](#other-practices)
- [Resources](#resources)
  - [Angular](#angular)
  - [TypeScript](#comments)
  - [Other Resources](#other-resources)
- [Windows Setup](#windows-setup)
  - [Tools](#tools)
  - [System](#system)
  - [Windows Subsystem Linux](#windows-subsystem-linux)
  - [Windows PowerShell](#windows-powershell)
  - [Git, Node, Npm](#git-node-npm)
  - [Docker](#docker)
  - [Google Chrome](#google-chrome)
  - [VS Code](#vs-code)
  - [Run Commands (.rc)](#run-commands)

# Community

## Gitter
- <strong><a href="https://gitter.im/" target="_blank" alt="gitter">Gitter</a></strong> - if you ever looked for a programmers chat where you could post a question and instantly get an answer (not like <a href="https://stackoverflow.com" target="_blank" alt="stackoverflow">stackoverflow</a>), I recommend joining channels: 
  - <strong><a href="https://gitter.im/Microsoft/TypeScript" target="_blank" alt="typescript gitter">TypeScript</a></strong>
  - <strong><a href="https://gitter.im/angular/angular" target="_blank" alt="angular gitter">Angular</a></strong>
  - <strong><a href="https://gitter.im/nodejs/node" target="_blank" alt="node gitter">Node.js</a></strong>

# Performance

## Loops
- Fastest loop:
```ts
for (let i = array.length - 1; i >= 0; --i) {

}
```
- `for of` better than `forEach`

## DOM
- `innerHTML` > `appendChild` (appendChild allows you to not lose events bound to DOM though)

# Practices

## Comments
- `// Start comments upperFirst with a dot in the end.`
- `/* Start comments upperFirst with a dot in the end. */`
- Place a line breaks before and after "comment block" except for return:
```ts
if (true) {

    // comment
    doSomething();

    // next comment
    doSomethingElse();

    // except for return
    return noLineBreakAfterMe();
}
```

## Naming
- **& vs And** - prefer "and", leave "&" for brand names and programming actions.
- **0.0.0 vs 1.0.0** - start development with `0.0.0` version, use `1.0.0` for first working release.
- **Add vs Create** - prefer "add". It's more intuitive for non-programmers.
- `app.js` **vs** `index.js` **vs** `main.js` **vs** `server.js`** - prefer `main.js` for an entry file, as it is chosen by Angular and NestJS. Leave index for `index.html` and default exporting via `index.js`.
- **Argument vs Parameter** - use params for method parameters, leave arguments for command line.
- **Async vs Defer** - prefer defer over async.
- **Attribute vs Property** - attribute for xml, properties for objects.
- **Change vs Modify vs Update** - prefer "update". It's more standard.
- **Common vs Partials vs Shared** - common for library names, shared for directory name, don't use partials.
- **Configuration vs Options vs Preferences vs Settings**
  - **Configuration** - for internal system (for example: `webpack.config.js`, `ecosystem.config.js`).
  - **Options** - for others choices (especially other developers, for example: `<radarsu-web-component options=""\>`).
  - **Settings** - for system-administrating end-user (for example: `admin dashboard`)
  - **Preferences** - for end-user (for example: `website visitor`).
- **Controller vs Resolver vs Route** - controller for REST, resolver for GraphQL, route for analysis of url, query and params and pointing to one of previously listed.
- **createdAt vs creationDate** - prefer "createdAt" over "creationDate". It's shorter and more common.
- **Delete vs Remove** - prefer "remove". It's more intuitive for non-programmers.
- **Demo vs Showcase** - prefer "showcase".
- **Entity vs Model** - use model, as it's part of MVC naming.
- **Helper, Handler, Manager** - don't use those at all. They carry no meaning.
- **Module vs Package** - module for internal stuff, package for external libraries.
- **Page vs View** - use view, as sometimes one page/view may be part of another one (also it's part of MVC).
- **Spec vs Test** - use spec, used by Angular and Google. Leave "test" for manual testing.
- **Node.js vs NodeJS** - Node.js, it's how it stands at their official page.

For general rules watch <a href="https://www.youtube.com/watch?v=CjOR5gCCZpk&feature=youtu.be&fbclid=IwAR08aUXhJ0AInlDnmIs2mnkPESOaro9B0hGFmMgVynQXbMvaVATE5o6If6U" target="_blank">How to name things in programming?</a>.

## Other Practices
- **Convention over Configuration** - prefer naming convetions over configuration of stuff. It often allows you to skip a lot of redundant code and data.
- **directory-naming** - use lowercase and dashes (kebab-case) for directory naming, never use `_` in directory naming. `.` is allowed for domain names.
- **Encoding** - utf8mb4_unicode_ci is the most correct.
- **Export everything** - when writing modules export almost everything except highly private functions. You never know what somebody would like to reuse or hack into.
- **File naming convention** - `file-name.scope.extension` (for example: `user.model.ts`, `news.controller.ts`).
- **Line length 150** is reasonable size (good for PC and laptops with 1920x1080 resolution). Eventually use 120.
- **Single method parameter** - prefer methods with single, complex parameter over multiple parameters - it's easier to refactor such method and keep backwards compatibility.
- **Port practices**
  - <1000, 1337, 3000, 4200, 8080-9999 - do not use those, they're commonly used.
  - 5001-5999 - production.
  - 6001-6999 - development.
  - 7001-7999 - testing.
- **Prefix interfaces** - prefer ISomeInterface over SomeInterface. TypeScript guidelines are against that, but that practice is actually very useful and stops you from common mistakes of trying to instantiate interfaces.
- **Use trailing commas** in arrays and after multiline object properties - it makes it easier to expand the code.
- **Use semicolons**, it's simply more popular (easier to copy code from documentations without need to adjust) and less error-prone.
- **Sort everything alphabetically** - When there is no certain logical order in elements, object keys or function call order.
- **Stay close to the metal** - do not make unnecessary wrappers, abstractions. If you use some library internally for example in an object constructor, allow passing configuration data to the library in an unchanged manner.
- `<strong><a>link</a></strong>` > `<a><strong>link</strong></a>`.

# Resources

## Angular
- <strong><a href="https://malcoded.com/posts/angular-fundamentals-modules" target="_blank" alt="angular modules explained">Angular Modules</a></strong> - definitions of angular modules `declaration`, `imports`, `providers` and `exports`.
- <strong><a href="https://itnext.io/choosing-a-highly-scalable-folder-structure-in-angular-d987de65ec7" target="_blank" alt="angular application structure">Application Structure</a></strong> - angular or any other module-based application directory structure.

## Typescript
- <strong><a href="https://github.com/torokmark/design_patterns_in_typescript" target="_blank" alt="typescript design patterns">Design patterns</a></strong>

## Other Resources
- <a href="http://chir.ag/projects/name-that-color/#722E75" target="_blank" alt="tool for color naming">Color naming</a>
- <strong><a href="https://graphql.org/learn/authorization/" target="_blank" alt="angular modules explained">GraphQL authorization</a></strong>
- <a href="https://tailwindcss.com/docs/" target="_blank" alt="utility first tailwind">Utility-first CSS</a> &gt; BEM vs SMACSS vs OOCSS

# Windows Setup

## Tools
- <a href="https://www.7-zip.org/" target="_blank">7-zip</a>
- <a href="https://download.docker.com/win/stable/Docker%20for%20Windows%20Installer.exe" target="_blank">Docker for Windows</a>
- <a href="https://filezilla-project.org/" target="_blank">Filezilla</a>
- <a href="https://www.google.com/intl/en/chrome/" target="_blank">Google Chrome</a>
- <a href="https://getgreenshot.org/" target="_blank">Greenshot</a>
- Microsoft Office
- <a href="https://www.mongodb.com/download-center/compass" target="_blank">MongoDB Compass</a>
- <a href="https://notepad-plus-plus.org/download/" target="_blank">Nodepad++</a> [set all text-files to be opened by default]
- <a href="https://www.getpostman.com/downloads/" target="_blank">Postman</a>
- <a href="https://github.com/Eugeny/terminus/releases/latest" target="_blank">Terminus</a>
- <a href="https://code.visualstudio.com/download/" target="_blank">VS Code</a>

### Optional
- <a href="https://www.bittorrent.com/lang/pl/">BitTorrent</a>
- <a href="https://discordapp.com/download" target="_blank">Discord</a>
- <a href="https://www.gimp.org/downloads/" target="_blank">GIMP</a>
- <a href="https://napiprojekt.pl/download/" target="_blank">NapiProjekt</a>
- <a href="http://plantuml.com/download">PlantUML</a>
- <a href="https://protonvpn.com/download/" target="_blank">ProtonVPN</a>
- <a href="https://slack.com/intl/en-de/downloads/windows">Slack</a>
- <a href="https://www.videolan.org/" target="_blank">VLC Media Player</a>

## System
- BIOS (F10 during system boot): enable Virtualization Technology (VT)
- <a href="https://www.fontsquirrel.com/fonts/fira-code" target="_blank">FiraCode Font</a>
- Windows Subsystem Linux Ubuntu (Microsoft Store)
- At `C:\Windows\System32\drivers\etc\hosts` add `127.0.0.1 localhost.radrat.pl`

## Windows Subsystem Linux
- `sudo apt install build-essential docker docker-compose make`

## Windows PowerShell
- Turn on Hyper-V for Docker: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All`

## Git, Node, Npm
`npm i -g @angular/cli @nestjs/schematics docusaurus-init eslint lerna lint-staged nodemon nps pm2 prettier prettier-eslint-cli ts-node tldr tslint typescript windows-build-tools webpack`

`npm login`

`git config --global user.name "Artur Kurowski"`

`git config --global user.email "radarsu@gmail.com"`

## Docker
- Settings: `Expose deamon on tcp://localhost:2375 without TLS`  

## Google Chrome
- <a href="https://chrome.google.com/webstore/detail/nodejs-v8-inspector-manag/gnhhdgbaldcilmgcpfddgdbkhjohddkj" target="_blank">Node Inspector Manager</a>
- <a href="https://chrome.google.com/webstore/detail/pop-up-blocker-for-chrome/bkkbcggnhapdmkeljlodobbkopceiche" target="_blank">Pop up blocker</a>
- <a href="https://chrome.google.com/webstore/detail/red-labels-for-pivotal-tr/agijkohaieagbidlmjjlajhlkpfoegao" target="_blank">Red Labels for Pivotal Tracker</a>
- <a href="https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd" target="_blank">Redux DevTools</a>
- <a href="https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo" target="_blank">Tampermonkey</a>
- <a href="https://chrome.google.com/webstore/detail/ublock-plus-adblocker/oofnbdifeelbaidfgpikinijekkjcicg" target="_blank">uBlock Plus Adblocker</a>
- <a href="https://chrome.google.com/webstore/detail/youtube-nonstop/nlkaejimjacpillmajjnopmpbkbnocid?hl=pl" target="_blank">YouTube NonStop</a>

## VS Code
- Better comments
- Bracker Pair Colorizer 2
- Browser Preview
- Cobalt2
- Docker
- Editorconfig for VS Code
- ESlint
- Gitlens
- GraphQL
- Markdown all in one
- Material Icon Theme
- Prettier
- Remote Development
- Sort js object keys
- Toggle quotes
- TSlint
- TypeScript Hero
 
## Run Commands
- .bashrc
  - Ending: 
```
# nvm
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion

# docker
export DOCKER_HOST=tcp://0.0.0.0:2375

# npm
export NPM_TOKEN="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
```
