# Jasmine
## VS Code Jasmine snippets
-------------------

<!-- [![Version](https://vsmarketplacebadge.apphb.com/version/xabikos.JasmineSnippets.svg)](https://marketplace.visualstudio.com/items?itemName=xabikos.JasmineSnippets) -->
<!-- [![Installs](https://vsmarketplacebadge.apphb.com/installs/xabikos.JasmineSnippets.svg)](https://marketplace.visualstudio.com/items?itemName=xabikos.JasmineSnippets) -->
<!-- [![Ratings](https://vsmarketplacebadge.apphb.com/rating/xabikos.JasmineSnippets.svg)](https://marketplace.visualstudio.com/items?itemName=xabikos.JasmineSnippets) -->

<!-- This extension contains code snippets for [Jasmine][jasmine] test framework and is based on the awesome [sublime-jasmine][sublime-jusmine] package by [@NicoSantangelo][NicoSantangelo]. -->

<!-- This extension is based on [xabios](https://github.com/xabikos), [JasmineSnippets](https://github.com/xabikos/vscode-jasmine). -->
<!-- I modified it according to the CODING STYLE GUIDE of my work, and I added some snippets that I use frequently. -->
This extension is based on [xabios'](https://github.com/xabikos) [JasmineSnippets](https://github.com/xabikos/vscode-jasmine) work .
I have modified it according to the Coding Style Guide that we use at work. I have also added some functions that I use very often.

## What is different?
* Single-quote is replaced by double-quote.

* I replaced this function:

| Trigger      | Content |
| -------:     | ------- |
| `desc→`      | describe method with nested it |

* I added these functions:

| Trigger      | Content |
| -------:     | ------- |
| `descb→`      | describe method with nested it and beforeEach |
| `descfull→`      | describe method with nested it, beforeEach and afterEach |

-*And adding an ‘a’:*

| Trigger      | Content |
| -------:     | ------- |
| `ita→`      | async it method |
| `desca→`      | describe method with nested async it |
| `descba→`      | describe method with nested async it and beforeEach |
| `descfulla→`      | describe method with nested async it, beforeEach and afterEach |

## Installation
This package isn’t in Visual Studio Marketplace. The easiest way to install it is with vsce.
To install in an Unix environment (tested with Debian):

1)- Clone the project:

`git clone https://github.com/jorgesarabia/vscode-jasmine.git`

2)- Install vsce globally with npm:

`npm install -g vsce`

3)- Package:

`cd vscode-jasmine`

`vsce package`

4)- Install it:

`code --install-extension JasmineSnippets-0.1.0.vsix`



## Supported languages (file extensions)
* JavaScript (.js)
* TypeScript (.ts)

## Snippets

Below is a list of all available snippets and the triggers of each one. The **→** means the `TAB` key.

### Specs
| Trigger      | Content |
| -------:     | ------- |
| `xdesc→`     | xdescribe method |
| `fdesc→`     | fdescribe method |
| `it→`        | it method |
| `xit→`       | xit method |
| `fit→`       | fit method |
| `ae→`        | after each method |
| `be→`        | before each method |

### Expectations
| Trigger  | Content |
| -------: | ------- |
| `exp→` 	 | expect |
| `tb→`    | expect().toBe |
| `tbct→`  | expect().toBeCloseTo |
| `tbd→`   | expect().toBeDefined |
| `tbf→`   | expect().toBeFalsy |
| `tbgt→`  | expect().toBeGreaterThan |
| `tblt→`  | expect().toBeLessThan |
| `tbn→`   | expect().toBeNull |
| `tbt→`   | expect().toBeTruthy |
| `tbu→`   | expect().toBeUndefined |
| `tc→`    | expect().toContain |
| `te→`    | expect().toEqual |
| `thbc→`  | expect().toHaveBeenCalled |
| `thbcw→` | expect().toHaveBeenCalledWith |
| `tm→`    | expect().toMatch |
| `tt→`    | expect().toThrow |
| `tte→`   | expect().toThrowError |
| `nb→`    | expect().not.toBe |
| `nct→`   | expect().not.toBeCloseTo |
| `nd→`    | expect().not.toBeDefined |
| `nf→`    | expect().not.toBeFalsy |
| `ngt→`   | expect().not.toBeGreaterThan |
| `nlt→`   | expect().not.toBeLessThan |
| `nn→`    | expect().not.toBeNull |
| `nt→`    | expect().not.toBeTruthy |
| `nu→`    | expect().not.toBeUndefined |
| `nc→`    | expect().not.toContain |
| `ne→`    | expect().not.toEqual |
| `nm→`    | expect().not.toMatch |
| `nt→`    | expect().not.toThrow |
| `any→`   | jasmine.any |
| `oc→`    | jasmine.objectContaining |

### Spies
| Trigger  | Content |
| -------: | ------- |
|`so→`     | spyOn |
|`sct→`    | spyOn.and.callThrough |
|`scf→`    | spyOn.and.callFake |
|`spg→`     | spyOnProperty($obj,'$property', 'get') |
|`sps→`     | spyOnProperty($obj,'$property', 'set') |
|`srv→`    | spyOn.and.returnValue |
|`ss→`     | spyOn.and.stub |
|`ste→`    | spyOn.and.throwError |
|`ca→`     | spy.calls.all |
|`caa→`    | spy.calls.allArgs |
|`ca→`     | spy.calls.any |
|`caf→`    | spy.calls.argsFor |
|`cc→`     | spy.calls.count |
|`cf→`     | spy.calls.first |
|`cmr→`    | spy.calls.mostRecent |
|`cr→`     | spy.calls.reset |
|`cs→`     | createSpy |
|`cso→`    | createSpyObj |

[jasmine]: http://jasmine.github.io
[sublime-jusmine]: https://github.com/NicoSantangelo/sublime-jasmine
[NicoSantangelo]: https://github.com/NicoSantangelo
