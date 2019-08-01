<p align="center">
    <a href="https://github.com/radarsu/me/" target="blank" alt="me"><img src="https://github.com/radarsu/me/blob/master/assets/logo.png?raw=true" alt="me logo" /></a><br/>
</p>

<p align="center">
	<strong>Personal version of <a href="https://github.com/sindresorhus/awesome" target="_blank" alt="awesome">Awesome</a> and best practices in short.</strong>
</p>

<p align="center">
	This repository purpose is to share resources interesting for TypeScript, Node.js and JavaScript full-stack developers.
</p>

## Description
Awesome repositories are usually targetted at certain things like - programming language, technology, books, etc. This one is composition of completely different stuff that's just personal, but might be useful for any full-stack developer interested in JavaScript, Node.js, Typescript and Angular.

## Community
- <strong><a href="https://gitter.im/" target="_blank" alt="gitter">Gitter</a></strong> - if you ever looked for a programmers chat where you could post a question and instantly get an answer (not like <a href="https://stackoverflow.com" target="_blank" alt="stackoverflow">stackoverflow</a>), I recommend joining channels: 
  - <strong><a href="https://gitter.im/Microsoft/TypeScript" target="_blank" alt="typescript gitter">TypeScript</a></strong>
  - <strong><a href="https://gitter.im/angular/angular" target="_blank" alt="angular gitter">Angular</a></strong>
  - <strong><a href="https://gitter.im/nodejs/node" target="_blank" alt="node gitter">Node.js</a></strong>

## Typescript
- <strong><a href="https://github.com/torokmark/design_patterns_in_typescript" target="_blank" alt="typescript design patterns">Design patterns</a></strong>.

## Node.js
  
## Angular
- <strong><a href="https://malcoded.com/posts/angular-fundamentals-modules" target="_blank" alt="angular modules explained">Angular Modules</a></strong> - definitions of angular modules `declaration`, `imports`, `providers` and `exports`.
- <strong><a href="https://itnext.io/choosing-a-highly-scalable-folder-structure-in-angular-d987de65ec7" target="_blank" alt="angular app structure">App structure</a></strong> - angular or any other module-based application directory structure.

## Practices
- `// short comments lowercase`
- `/* Start comments upperFirst with a dot in the end. */`
- Place a line breaks before and after "comment block":
```ts
if (true) {

	// comment
	doSomething();

	// next comment
	doSomethingElse();

}
```
- <strong><a href="https://graphql.org/learn/authorization/" target="_blank" alt="angular modules explained">GraphQL authorization</a></strong>
- <a href="https://tailwindcss.com/docs/" target="_blank" alt="utility first tailwind">Utility-first CSS</a> &gt; BEM vs SMACSS vs OOCSS
- <a href="http://chir.ag/projects/name-that-color/#722E75" target="_blank" alt="tool for color naming">Color naming</a>

## Naming
- <strong>Attribute vs Property</strong> - attribute for xml, properties for objects.
- <strong>Common vs Shared vs Partials</strong> - common for library names, shared for directory name, don't use partials.
- <strong>Controller vs Resolver vs Route</strong> - controller for REST, resolver for GraphQL, route for analysis of url, query and params and pointing to one of previously listed.
- <strong>Entity vs Model</strong> - entity for instances, model for coded stuff.
- <strong>Module vs Package</strong> - module for internal stuff, package for external libraries.
- <strong>Page vs View</strong> - use view, as sometimes one page/view may be part of another one.

## Performance
- Fastest loop:
```ts
for (let i = array.length - 1; i >= 0; --i) {

}
```
- `for of` better than `forEach`

## DOM
- appendChild better than innerHTML only if you don't want content to lose events etc., innerHTML overall better for whole content rendering

# Windows Initial Setup

## Utility
  - <a href="https://www.7-zip.org/" target="_blank">7-zip</a>
  - <a href="https://filezilla-project.org/" target="_blank">Filezilla</a>
  - <a href="https://www.google.com/intl/en/chrome/" target="_blank">Google Chrome</a>
  - <a href="https://getgreenshot.org/" target="_blank">Greenshot</a>
  - Microsoft Office
  - <a href="https://www.videolan.org/" target="_blank">VLC Media Player</a>

## System
  - BIOS (F10 during system boot): enable Virtualization Technology (VT)
  - <a href="https://www.fontsquirrel.com/fonts/fira-code" target="_blank">FiraCode Font</a>
  - Windows Subsystem Linux Ubuntu (Microsoft Store)

## Windows Subsystem Linux
  - `sudo apt install build-essential docker docker-compose make`
  - zsh, slimzsh & oh my zsh
  
## Windows PowerShell
  - Turn on Hyper-V for Docker: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All`

## Development
  - <a href="https://download.docker.com/win/stable/Docker%20for%20Windows%20Installer.exe" target="_blank">Docker for Windows</a>
  - <a href="https://notepad-plus-plus.org/download/" target="_blank">Nodepad++</a> [set all text-files to be opened by default]
  - <a href="https://code.visualstudio.com/insiders/" target="_blank">VS CODE Insiders</a>

## Git, Node & Npm
  - `npm i -g eslint lerna nodemon nps pm2 ts-node tslint typescript webpack`
  - `npm login`
  - `git config --global user.name "Artur Kurowski"`
  - `git config --global user.email "radarsu@gmail.com"`

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
  
## Run Commands (.rc)
  - .zshrc
    - Ending: 
```
# nvm
[[ -s $HOME/.nvm/nvm.sh ]] && . $HOME/.nvm/nvm.sh

# docker
export DOCKER_HOST=localhost:2375

# npm
export NPM_TOKEN="23c31450-5b72-4479-bde3-4e5df50da2d9"
```
