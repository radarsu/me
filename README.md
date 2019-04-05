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
- <strong><a href="https://graphql.org/learn/authorization/" target="_blank" alt="angular modules explained">GraphQL authorization</a></strong>
- <a href="https://tailwindcss.com/docs/" target="_blank" alt="utility first tailwind">Utility-first CSS</a> &gt; BEM vs SMACSS vs OOCSS.
- <a href="http://chir.ag/projects/name-that-color/#722E75" target="_blank" alt="tool for color naming">Color naming</a>.

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
