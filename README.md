<p align="center">
    <a href="https://github.com/radarsu/me/" target="blank" alt="me"><img src="https://github.com/radarsu/me/blob/master/assets/logo.png?raw=true" alt="me logo" /></a><br/>
</p>

<p align="center">
	<strong>Personal version of <a href="https://github.com/sindresorhus/awesome" target="_blank" alt="awesome">Awesome</a>.</strong>
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

## Node.js
  
## Angular
- <strong><a href="https://malcoded.com/posts/angular-fundamentals-modules" target="_blank" alt="angular modules explained">Angular Modules</a></strong> - definitions of angular modules `declaration`, `imports`, `providers` and `exports`.
- <strong><a href="https://itnext.io/choosing-a-highly-scalable-folder-structure-in-angular-d987de65ec7" target="_blank" alt="angular app structure">App structure</a></strong> - angular or any other module-based application directory structure.

## Practices
- <strong>Shared vs Common</strong> - shared for directory name, common for library names.
- `// short comments lowercase`
- `/* Star comments upperFirst with a dot in the end. */`
- Place a line breaks before and after "comment block":
```ts
if (true) {

	// comment
	doSomething();

	// next comment
	doSomethingElse();

}
```

## Performance
- Fastest loop:
```ts
for (let i = array.length - 1; i >= 0; --i) {

}
```
- `for of` better than `forEach`
- DOM:
  - appendChild better than innerHTML for small number of items, innerHTML overall better for whole content rendering
