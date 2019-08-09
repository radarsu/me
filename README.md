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
- `// short comments lowercase`
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
- **& vs And** - always use "and", leave "&" for brand names and programming.
- **Attribute vs Property** - attribute for xml, properties for objects.
- **Common vs Shared vs Partials** - common for library names, shared for directory name, don't use partials.
- **Configuration vs Options vs Preferences vs Settings**
  - **Configuration** - for internal system (for example: `webpack.config.js`, `ecosystem.config.js`).
  - **Options** - for others choices (especially other developers, for example: `<radarsu-web-component options=""\>`).
  - **Settings** - for system-administrating end-user (for example: `admin dashboard`)
  - **Preferences** - for end-user (for example: `website visitor`).
- **Controller vs Resolver vs Route** - controller for REST, resolver for GraphQL, route for analysis of url, query and params and pointing to one of previously listed.
- **Entity vs Model** - use model, as it's part of MVC naming.
- **Module vs Package** - module for internal stuff, package for external libraries.
- **Page vs View** - use view, as sometimes one page/view may be part of another one (also it's part of MVC).
- **Node.js vs NodeJS** - Node.js, it's how it stands at their official page.

## Other Practices
- **Convention over Configuration** - prefer naming convetions over configuration of stuff. It often allows you to skip a lot of redundant code and data.
- **directory-naming** - use lowercase and dashes (kebab-case) for directory naming, never use `_` or `.` in directory naming.
- **file.naming.convention** - `file-name.scope.extension` (for example: `user.model.ts`, `news.controller.ts`).
- **Line length 120** is reasonable size (good for PC and laptops with 1920x1080 resolution).
- **Use trailing commas** in arrays and after multiline object properties - it makes it easier to expand the code.
- **Use semicolons**, it's simply more popular (easier to copy code from documentations without need to adjust) and less error-prone.
- **Sort everything alphabetically** - When there is no certain logical order in elements, object keys or function call order.
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
- <a href="https://discordapp.com/download" target="_blank">Discord</a>
- <a href="https://download.docker.com/win/stable/Docker%20for%20Windows%20Installer.exe" target="_blank">Docker for Windows</a>
- <a href="https://filezilla-project.org/" target="_blank">Filezilla</a>
- <a href="https://www.google.com/intl/en/chrome/" target="_blank">Google Chrome</a>
- <a href="https://getgreenshot.org/" target="_blank">Greenshot</a>
- Microsoft Office
- <a href="https://downloads.mongodb.com/compass/mongodb-compass-1.18.0-win32-x64.msi" target="_blank">MongoDB Compass (win-64bit)</a>
- <a href="https://notepad-plus-plus.org/download/" target="_blank">Nodepad++</a> [set all text-files to be opened by default]
- <a href="https://www.getpostman.com/downloads/" target="_blank">Postman</a>
- <a href="https://code.visualstudio.com/insiders/" target="_blank">VS CODE Insiders</a>

### Fun/Optional
- <a href="https://napiprojekt.pl/download/" target="_blank">NapiProjekt</a>
- <a href="http://plantuml.com/download">PlantUML</a>
- <a href="https://www.videolan.org/" target="_blank">VLC Media Player</a>

## System
- BIOS (F10 during system boot): enable Virtualization Technology (VT)
- <a href="https://www.fontsquirrel.com/fonts/fira-code" target="_blank">FiraCode Font</a>
- Windows Subsystem Linux Ubuntu (Microsoft Store)

## Windows Subsystem Linux
- `sudo apt install build-essential docker docker-compose make`

## Windows PowerShell
- Turn on Hyper-V for Docker: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All`

## Git, Node, Npm
`npm i -g eslint lerna lint-staged nodemon nps pm2 prettier prettier-eslint-cli ts-node tldr tslint typescript windows-build-tools webpack`

`npm login`

`git config --global user.name "Artur Kurowski"`

`git config --global user.email "radarsu@gmail.com"`

## Docker
- Settings: `Expose deamon on tcp://localhost:2375 without TLS`  

## VS Code
- Better comments
- Bracker Pair Colorizer 2
- Cobalt2
- ESlint
- Gitlens
- Markdown all in one
- Material Icon Theme
- Prettier
- Remove Development
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
export DOCKER_HOST=localhost:2375

# npm
export NPM_TOKEN="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
```
