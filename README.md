
<div align="center">
    <h1><a href="https://github.com/hlsiira/Flux">Flux</a> - A simplistic (ES6) library for Event Delegation.</h1>
</div>

<div align="center">

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

</div>

## About
Flux is a compact library for creating individual event listeners while efficiently reducing processing overhead via Event Delegation, built off of <a href="https://github.com/cferdinandi/events">Chris Ferdinandi's Events</a>. Weighing in at under <b>150 lines</b> of code, Flux was built in order to be used as a compact and intuitive Event Delegation library for development on the <a href="https://www.athos.io/">Atheos IDE</a>, however it's proved so valuable as to become it's own mini library.

To learn more aboue Event Delegation, check out Chris' blog [here](https://gomakethings.com/checking-event-target-selectors-with-event-bubbling-in-vanilla-javascript/)

## Features
<p><code>Pleasently Parsed:</code> Flux automatically tries to parse JSON replies.</p>
<p><code>Crazily Condensed:</code> The minified version is less than ~1K, roughly 500b gzipped.</p>
<p><code>Easily Extensible:</code> Flux is easily modifyable to meet your needs.</p>

Below are the functions returned as an object when creating a new Flux refence.
```javascript
fX('#selector'){
	exists: (s) => exists(s),
	list: () => list(s),
	off: (t, fn) => off(t, s, fn),
	on: (t, fn) => on(t, s, fn),
	once: (t, fn) => once(t, s, fn),
	reset: () => reset(s),
	trigger: (e, o) => trigger(s, e, o)
}
```