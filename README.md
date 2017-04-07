# api documentation for  [regenerator (v0.9.7)](http://github.com/facebook/regenerator)  [![npm package](https://img.shields.io/npm/v/npmdoc-regenerator.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-regenerator) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-regenerator.svg)](https://travis-ci.org/npmdoc/node-npmdoc-regenerator)
#### Source transformer enabling ECMAScript 6 generator functions (yield) in JavaScript-of-today (ES5)

[![NPM](https://nodei.co/npm/regenerator.png?downloads=true)](https://www.npmjs.com/package/regenerator)

[![apidoc](https://npmdoc.github.io/node-npmdoc-regenerator/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-regenerator_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-regenerator/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-regenerator/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-regenerator/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Ben Newman",
        "email": "bn@cs.stanford.edu"
    },
    "bin": {
        "regenerator": "bin/regenerator"
    },
    "bugs": {
        "url": "https://github.com/facebook/regenerator/issues"
    },
    "dependencies": {
        "babel-core": "^6.18.2",
        "commoner": "^0.10.8",
        "recast": "^0.11.17",
        "regenerator-preset": "^0.9.6",
        "regenerator-runtime": "^0.10.3",
        "through": "^2.3.8"
    },
    "description": "Source transformer enabling ECMAScript 6 generator functions (yield) in JavaScript-of-today (ES5)",
    "devDependencies": {
        "babylon": "^6.14.1",
        "mocha": "^2.3.4",
        "promise": "^7.0.4",
        "semver": "^5.0.3"
    },
    "directories": {},
    "dist": {
        "shasum": "e0ba58ebbde23b896eac75ae7b93be2483ccf86f",
        "tarball": "https://registry.npmjs.org/regenerator/-/regenerator-0.9.7.tgz"
    },
    "engines": {
        "node": ">= 0.6"
    },
    "gitHead": "c7207b0f673f229f44e0d9174a65607c1b975131",
    "homepage": "http://github.com/facebook/regenerator",
    "keywords": [
        "generator",
        "yield",
        "coroutine",
        "rewriting",
        "transformation",
        "syntax",
        "codegen",
        "rewriting",
        "refactoring",
        "transpiler",
        "desugaring",
        "ES6"
    ],
    "license": "BSD",
    "main": "main.js",
    "maintainers": [
        {
            "name": "benjamn",
            "email": "bn@cs.stanford.edu"
        }
    ],
    "name": "regenerator",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/facebook/regenerator.git"
    },
    "scripts": {
        "pretest": "./link.sh",
        "test": "node test/run.js"
    },
    "version": "0.9.7"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module regenerator](#apidoc.module.regenerator)
1.  [function <span class="apidocSignatureSpan">regenerator.</span>compile (source, options)](#apidoc.element.regenerator.compile)
1.  [function <span class="apidocSignatureSpan">regenerator.</span>runtime ()](#apidoc.element.regenerator.runtime)
1.  [function <span class="apidocSignatureSpan">regenerator.</span>transform (node, options)](#apidoc.element.regenerator.transform)
1.  [function <span class="apidocSignatureSpan">regenerator.</span>types.NodePath (value, parentPath, name)](#apidoc.element.regenerator.types.NodePath)
1.  [function <span class="apidocSignatureSpan">regenerator.</span>types.Path (value, parentPath, name)](#apidoc.element.regenerator.types.Path)
1.  [function <span class="apidocSignatureSpan">regenerator.</span>types.PathVisitor ()](#apidoc.element.regenerator.types.PathVisitor)
1.  [function <span class="apidocSignatureSpan">regenerator.</span>types.Type (check, name)](#apidoc.element.regenerator.types.Type)
1.  [function <span class="apidocSignatureSpan">regenerator.</span>types.astNodesAreEquivalent (a, b, problemPath)](#apidoc.element.regenerator.types.astNodesAreEquivalent)
1.  object <span class="apidocSignatureSpan">regenerator.</span>runtime_module
1.  object <span class="apidocSignatureSpan">regenerator.</span>types
1.  object <span class="apidocSignatureSpan">regenerator.</span>types.NodePath.prototype
1.  object <span class="apidocSignatureSpan">regenerator.</span>types.Path.prototype
1.  object <span class="apidocSignatureSpan">regenerator.</span>types.PathVisitor.prototype
1.  object <span class="apidocSignatureSpan">regenerator.</span>types.Type.prototype
1.  object <span class="apidocSignatureSpan">regenerator.</span>types.builders
1.  object <span class="apidocSignatureSpan">regenerator.</span>util
1.  object <span class="apidocSignatureSpan">regenerator.</span>visit

#### [module regenerator.runtime_module](#apidoc.module.regenerator.runtime_module)
1.  [function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>AsyncIterator (generator)](#apidoc.element.regenerator.runtime_module.AsyncIterator)
1.  [function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>async (innerFn, outerFn, self, tryLocsList)](#apidoc.element.regenerator.runtime_module.async)
1.  [function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>awrap (arg)](#apidoc.element.regenerator.runtime_module.awrap)
1.  [function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>isGeneratorFunction (genFun)](#apidoc.element.regenerator.runtime_module.isGeneratorFunction)
1.  [function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>keys (object)](#apidoc.element.regenerator.runtime_module.keys)
1.  [function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>mark (genFun)](#apidoc.element.regenerator.runtime_module.mark)
1.  [function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>values (iterable)](#apidoc.element.regenerator.runtime_module.values)
1.  [function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>wrap (innerFn, outerFn, self, tryLocsList)](#apidoc.element.regenerator.runtime_module.wrap)

#### [module regenerator.types](#apidoc.module.regenerator.types)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>NodePath (value, parentPath, name)](#apidoc.element.regenerator.types.NodePath)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>Path (value, parentPath, name)](#apidoc.element.regenerator.types.Path)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>PathVisitor ()](#apidoc.element.regenerator.types.PathVisitor)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>Type (check, name)](#apidoc.element.regenerator.types.Type)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>astNodesAreEquivalent (a, b, problemPath)](#apidoc.element.regenerator.types.astNodesAreEquivalent)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>defineMethod (name, func)](#apidoc.element.regenerator.types.defineMethod)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>eachField (object, callback, context)](#apidoc.element.regenerator.types.eachField)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>finalize ()](#apidoc.element.regenerator.types.finalize)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>getFieldNames (object)](#apidoc.element.regenerator.types.getFieldNames)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>getFieldValue (object, fieldName)](#apidoc.element.regenerator.types.getFieldValue)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>getSupertypeNames (typeName)](#apidoc.element.regenerator.types.getSupertypeNames)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>someField (object, callback, context)](#apidoc.element.regenerator.types.someField)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>use (plugin)](#apidoc.element.regenerator.types.use)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>visit (node, methods)](#apidoc.element.regenerator.types.visit)
1.  object <span class="apidocSignatureSpan">regenerator.types.</span>builders
1.  object <span class="apidocSignatureSpan">regenerator.types.</span>builtInTypes
1.  object <span class="apidocSignatureSpan">regenerator.types.</span>namedTypes

#### [module regenerator.types.NodePath](#apidoc.module.regenerator.types.NodePath)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>NodePath (value, parentPath, name)](#apidoc.element.regenerator.types.NodePath.NodePath)

#### [module regenerator.types.NodePath.prototype](#apidoc.module.regenerator.types.NodePath.prototype)
1.  [function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>_computeNode ()](#apidoc.element.regenerator.types.NodePath.prototype._computeNode)
1.  [function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>_computeParent ()](#apidoc.element.regenerator.types.NodePath.prototype._computeParent)
1.  [function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>_computeScope ()](#apidoc.element.regenerator.types.NodePath.prototype._computeScope)
1.  [function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>canBeFirstInStatement ()](#apidoc.element.regenerator.types.NodePath.prototype.canBeFirstInStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>firstInStatement ()](#apidoc.element.regenerator.types.NodePath.prototype.firstInStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>getValueProperty (name)](#apidoc.element.regenerator.types.NodePath.prototype.getValueProperty)
1.  [function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>needsParens (assumeExpressionContext)](#apidoc.element.regenerator.types.NodePath.prototype.needsParens)
1.  [function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>prune ()](#apidoc.element.regenerator.types.NodePath.prototype.prune)
1.  [function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>replace ()](#apidoc.element.regenerator.types.NodePath.prototype.replace)

#### [module regenerator.types.Path](#apidoc.module.regenerator.types.Path)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>Path (value, parentPath, name)](#apidoc.element.regenerator.types.Path.Path)

#### [module regenerator.types.Path.prototype](#apidoc.module.regenerator.types.Path.prototype)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>each (callback, context)](#apidoc.element.regenerator.types.Path.prototype.each)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>filter (callback, context)](#apidoc.element.regenerator.types.Path.prototype.filter)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>get (name)](#apidoc.element.regenerator.types.Path.prototype.get)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>getValueProperty (name)](#apidoc.element.regenerator.types.Path.prototype.getValueProperty)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>insertAfter (node)](#apidoc.element.regenerator.types.Path.prototype.insertAfter)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>insertAt (index, node)](#apidoc.element.regenerator.types.Path.prototype.insertAt)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>insertBefore (node)](#apidoc.element.regenerator.types.Path.prototype.insertBefore)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>map (callback, context)](#apidoc.element.regenerator.types.Path.prototype.map)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>pop ()](#apidoc.element.regenerator.types.Path.prototype.pop)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>push (node)](#apidoc.element.regenerator.types.Path.prototype.push)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>replace (replacement)](#apidoc.element.regenerator.types.Path.prototype.replace)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>shift ()](#apidoc.element.regenerator.types.Path.prototype.shift)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>unshift (node)](#apidoc.element.regenerator.types.Path.prototype.unshift)

#### [module regenerator.types.PathVisitor](#apidoc.module.regenerator.types.PathVisitor)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>PathVisitor ()](#apidoc.element.regenerator.types.PathVisitor.PathVisitor)
1.  [function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.</span>fromMethodsObject (methods)](#apidoc.element.regenerator.types.PathVisitor.fromMethodsObject)
1.  [function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.</span>visit (node, methods)](#apidoc.element.regenerator.types.PathVisitor.visit)

#### [module regenerator.types.PathVisitor.prototype](#apidoc.module.regenerator.types.PathVisitor.prototype)
1.  [function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>AbortRequest ()](#apidoc.element.regenerator.types.PathVisitor.prototype.AbortRequest)
1.  [function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>abort ()](#apidoc.element.regenerator.types.PathVisitor.prototype.abort)
1.  [function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>acquireContext (path)](#apidoc.element.regenerator.types.PathVisitor.prototype.acquireContext)
1.  [function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>releaseContext (context)](#apidoc.element.regenerator.types.PathVisitor.prototype.releaseContext)
1.  [function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>reportChanged ()](#apidoc.element.regenerator.types.PathVisitor.prototype.reportChanged)
1.  [function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>reset (path)](#apidoc.element.regenerator.types.PathVisitor.prototype.reset)
1.  [function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>visit ()](#apidoc.element.regenerator.types.PathVisitor.prototype.visit)
1.  [function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>visitWithoutReset (path)](#apidoc.element.regenerator.types.PathVisitor.prototype.visitWithoutReset)
1.  [function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>wasChangeReported ()](#apidoc.element.regenerator.types.PathVisitor.prototype.wasChangeReported)

#### [module regenerator.types.Type](#apidoc.module.regenerator.types.Type)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>Type (check, name)](#apidoc.element.regenerator.types.Type.Type)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Type.</span>def (typeName)](#apidoc.element.regenerator.types.Type.def)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Type.</span>fromArray (arr)](#apidoc.element.regenerator.types.Type.fromArray)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Type.</span>fromObject (obj)](#apidoc.element.regenerator.types.Type.fromObject)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Type.</span>or ()](#apidoc.element.regenerator.types.Type.or)

#### [module regenerator.types.Type.prototype](#apidoc.module.regenerator.types.Type.prototype)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Type.prototype.</span>arrayOf ()](#apidoc.element.regenerator.types.Type.prototype.arrayOf)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Type.prototype.</span>assert (value, deep)](#apidoc.element.regenerator.types.Type.prototype.assert)
1.  [function <span class="apidocSignatureSpan">regenerator.types.Type.prototype.</span>toString ()](#apidoc.element.regenerator.types.Type.prototype.toString)

#### [module regenerator.types.astNodesAreEquivalent](#apidoc.module.regenerator.types.astNodesAreEquivalent)
1.  [function <span class="apidocSignatureSpan">regenerator.types.</span>astNodesAreEquivalent (a, b, problemPath)](#apidoc.element.regenerator.types.astNodesAreEquivalent.astNodesAreEquivalent)
1.  [function <span class="apidocSignatureSpan">regenerator.types.astNodesAreEquivalent.</span>assert (a, b)](#apidoc.element.regenerator.types.astNodesAreEquivalent.assert)

#### [module regenerator.types.builders](#apidoc.module.regenerator.types.builders)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>anyTypeAnnotation ()](#apidoc.element.regenerator.types.builders.anyTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>arrayExpression ()](#apidoc.element.regenerator.types.builders.arrayExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>arrayPattern ()](#apidoc.element.regenerator.types.builders.arrayPattern)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>arrayStatement ()](#apidoc.element.regenerator.types.builders.arrayStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>arrayTypeAnnotation ()](#apidoc.element.regenerator.types.builders.arrayTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>arrowFunctionExpression ()](#apidoc.element.regenerator.types.builders.arrowFunctionExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>arrowFunctionStatement ()](#apidoc.element.regenerator.types.builders.arrowFunctionStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>assignmentExpression ()](#apidoc.element.regenerator.types.builders.assignmentExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>assignmentPattern ()](#apidoc.element.regenerator.types.builders.assignmentPattern)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>assignmentStatement ()](#apidoc.element.regenerator.types.builders.assignmentStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>awaitExpression ()](#apidoc.element.regenerator.types.builders.awaitExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>awaitStatement ()](#apidoc.element.regenerator.types.builders.awaitStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>binaryExpression ()](#apidoc.element.regenerator.types.builders.binaryExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>binaryStatement ()](#apidoc.element.regenerator.types.builders.binaryStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>bindExpression ()](#apidoc.element.regenerator.types.builders.bindExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>bindStatement ()](#apidoc.element.regenerator.types.builders.bindStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>block ()](#apidoc.element.regenerator.types.builders.block)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>blockStatement ()](#apidoc.element.regenerator.types.builders.blockStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>booleanLiteral ()](#apidoc.element.regenerator.types.builders.booleanLiteral)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>booleanLiteralStatement ()](#apidoc.element.regenerator.types.builders.booleanLiteralStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>booleanLiteralTypeAnnotation ()](#apidoc.element.regenerator.types.builders.booleanLiteralTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>booleanTypeAnnotation ()](#apidoc.element.regenerator.types.builders.booleanTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>breakStatement ()](#apidoc.element.regenerator.types.builders.breakStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>callExpression ()](#apidoc.element.regenerator.types.builders.callExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>callStatement ()](#apidoc.element.regenerator.types.builders.callStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>catchClause ()](#apidoc.element.regenerator.types.builders.catchClause)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classBody ()](#apidoc.element.regenerator.types.builders.classBody)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classDeclaration ()](#apidoc.element.regenerator.types.builders.classDeclaration)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classExpression ()](#apidoc.element.regenerator.types.builders.classExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classImplements ()](#apidoc.element.regenerator.types.builders.classImplements)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classMethod ()](#apidoc.element.regenerator.types.builders.classMethod)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classProperty ()](#apidoc.element.regenerator.types.builders.classProperty)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classPropertyDefinition ()](#apidoc.element.regenerator.types.builders.classPropertyDefinition)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classStatement ()](#apidoc.element.regenerator.types.builders.classStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>commentBlock ()](#apidoc.element.regenerator.types.builders.commentBlock)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>commentLine ()](#apidoc.element.regenerator.types.builders.commentLine)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>comprehensionBlock ()](#apidoc.element.regenerator.types.builders.comprehensionBlock)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>comprehensionExpression ()](#apidoc.element.regenerator.types.builders.comprehensionExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>comprehensionStatement ()](#apidoc.element.regenerator.types.builders.comprehensionStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>conditionalExpression ()](#apidoc.element.regenerator.types.builders.conditionalExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>conditionalStatement ()](#apidoc.element.regenerator.types.builders.conditionalStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>continueStatement ()](#apidoc.element.regenerator.types.builders.continueStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>debuggerStatement ()](#apidoc.element.regenerator.types.builders.debuggerStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareClass ()](#apidoc.element.regenerator.types.builders.declareClass)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareExportAllDeclaration ()](#apidoc.element.regenerator.types.builders.declareExportAllDeclaration)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareExportDeclaration ()](#apidoc.element.regenerator.types.builders.declareExportDeclaration)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareFunction ()](#apidoc.element.regenerator.types.builders.declareFunction)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareInterface ()](#apidoc.element.regenerator.types.builders.declareInterface)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareModule ()](#apidoc.element.regenerator.types.builders.declareModule)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareModuleExports ()](#apidoc.element.regenerator.types.builders.declareModuleExports)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareTypeAlias ()](#apidoc.element.regenerator.types.builders.declareTypeAlias)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareVariable ()](#apidoc.element.regenerator.types.builders.declareVariable)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>decorator ()](#apidoc.element.regenerator.types.builders.decorator)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>directive ()](#apidoc.element.regenerator.types.builders.directive)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>directiveLiteral ()](#apidoc.element.regenerator.types.builders.directiveLiteral)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>directiveLiteralStatement ()](#apidoc.element.regenerator.types.builders.directiveLiteralStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>doExpression ()](#apidoc.element.regenerator.types.builders.doExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>doStatement ()](#apidoc.element.regenerator.types.builders.doStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>doWhileStatement ()](#apidoc.element.regenerator.types.builders.doWhileStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>emptyStatement ()](#apidoc.element.regenerator.types.builders.emptyStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>emptyTypeAnnotation ()](#apidoc.element.regenerator.types.builders.emptyTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>existentialTypeParam ()](#apidoc.element.regenerator.types.builders.existentialTypeParam)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>existsTypeAnnotation ()](#apidoc.element.regenerator.types.builders.existsTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportAllDeclaration ()](#apidoc.element.regenerator.types.builders.exportAllDeclaration)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportBatchSpecifier ()](#apidoc.element.regenerator.types.builders.exportBatchSpecifier)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportDeclaration ()](#apidoc.element.regenerator.types.builders.exportDeclaration)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportDefaultDeclaration ()](#apidoc.element.regenerator.types.builders.exportDefaultDeclaration)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportDefaultSpecifier ()](#apidoc.element.regenerator.types.builders.exportDefaultSpecifier)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportNamedDeclaration ()](#apidoc.element.regenerator.types.builders.exportNamedDeclaration)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportNamespaceSpecifier ()](#apidoc.element.regenerator.types.builders.exportNamespaceSpecifier)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportSpecifier ()](#apidoc.element.regenerator.types.builders.exportSpecifier)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>expressionStatement ()](#apidoc.element.regenerator.types.builders.expressionStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>file ()](#apidoc.element.regenerator.types.builders.file)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>forAwaitStatement ()](#apidoc.element.regenerator.types.builders.forAwaitStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>forInStatement ()](#apidoc.element.regenerator.types.builders.forInStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>forOfStatement ()](#apidoc.element.regenerator.types.builders.forOfStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>forStatement ()](#apidoc.element.regenerator.types.builders.forStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>functionDeclaration ()](#apidoc.element.regenerator.types.builders.functionDeclaration)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>functionExpression ()](#apidoc.element.regenerator.types.builders.functionExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>functionStatement ()](#apidoc.element.regenerator.types.builders.functionStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>functionTypeAnnotation ()](#apidoc.element.regenerator.types.builders.functionTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>functionTypeParam ()](#apidoc.element.regenerator.types.builders.functionTypeParam)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>generatorExpression ()](#apidoc.element.regenerator.types.builders.generatorExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>generatorStatement ()](#apidoc.element.regenerator.types.builders.generatorStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>genericTypeAnnotation ()](#apidoc.element.regenerator.types.builders.genericTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>graphExpression ()](#apidoc.element.regenerator.types.builders.graphExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>graphIndexExpression ()](#apidoc.element.regenerator.types.builders.graphIndexExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>graphIndexStatement ()](#apidoc.element.regenerator.types.builders.graphIndexStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>graphStatement ()](#apidoc.element.regenerator.types.builders.graphStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>identifier ()](#apidoc.element.regenerator.types.builders.identifier)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>identifierStatement ()](#apidoc.element.regenerator.types.builders.identifierStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>ifStatement ()](#apidoc.element.regenerator.types.builders.ifStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>import ()](#apidoc.element.regenerator.types.builders.import)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>importDeclaration ()](#apidoc.element.regenerator.types.builders.importDeclaration)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>importDefaultSpecifier ()](#apidoc.element.regenerator.types.builders.importDefaultSpecifier)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>importNamespaceSpecifier ()](#apidoc.element.regenerator.types.builders.importNamespaceSpecifier)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>importSpecifier ()](#apidoc.element.regenerator.types.builders.importSpecifier)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>importStatement ()](#apidoc.element.regenerator.types.builders.importStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>interfaceDeclaration ()](#apidoc.element.regenerator.types.builders.interfaceDeclaration)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>interfaceExtends ()](#apidoc.element.regenerator.types.builders.interfaceExtends)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>intersectionTypeAnnotation ()](#apidoc.element.regenerator.types.builders.intersectionTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxAttribute ()](#apidoc.element.regenerator.types.builders.jsxAttribute)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxClosingElement ()](#apidoc.element.regenerator.types.builders.jsxClosingElement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxElement ()](#apidoc.element.regenerator.types.builders.jsxElement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxElementStatement ()](#apidoc.element.regenerator.types.builders.jsxElementStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxEmptyExpression ()](#apidoc.element.regenerator.types.builders.jsxEmptyExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxEmptyStatement ()](#apidoc.element.regenerator.types.builders.jsxEmptyStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxExpressionContainer ()](#apidoc.element.regenerator.types.builders.jsxExpressionContainer)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxExpressionContainerStatement ()](#apidoc.element.regenerator.types.builders.jsxExpressionContainerStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxIdentifier ()](#apidoc.element.regenerator.types.builders.jsxIdentifier)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxIdentifierStatement ()](#apidoc.element.regenerator.types.builders.jsxIdentifierStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxMemberExpression ()](#apidoc.element.regenerator.types.builders.jsxMemberExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxMemberStatement ()](#apidoc.element.regenerator.types.builders.jsxMemberStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxNamespacedName ()](#apidoc.element.regenerator.types.builders.jsxNamespacedName)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxOpeningElement ()](#apidoc.element.regenerator.types.builders.jsxOpeningElement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxSpreadAttribute ()](#apidoc.element.regenerator.types.builders.jsxSpreadAttribute)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxText ()](#apidoc.element.regenerator.types.builders.jsxText)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxTextStatement ()](#apidoc.element.regenerator.types.builders.jsxTextStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>labeledStatement ()](#apidoc.element.regenerator.types.builders.labeledStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>letExpression ()](#apidoc.element.regenerator.types.builders.letExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>letStatement ()](#apidoc.element.regenerator.types.builders.letStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>line ()](#apidoc.element.regenerator.types.builders.line)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>literal ()](#apidoc.element.regenerator.types.builders.literal)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>literalStatement ()](#apidoc.element.regenerator.types.builders.literalStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>logicalExpression ()](#apidoc.element.regenerator.types.builders.logicalExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>logicalStatement ()](#apidoc.element.regenerator.types.builders.logicalStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>memberExpression ()](#apidoc.element.regenerator.types.builders.memberExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>memberStatement ()](#apidoc.element.regenerator.types.builders.memberStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>memberTypeAnnotation ()](#apidoc.element.regenerator.types.builders.memberTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>metaProperty ()](#apidoc.element.regenerator.types.builders.metaProperty)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>metaPropertyStatement ()](#apidoc.element.regenerator.types.builders.metaPropertyStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>methodDefinition ()](#apidoc.element.regenerator.types.builders.methodDefinition)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>mixedTypeAnnotation ()](#apidoc.element.regenerator.types.builders.mixedTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>newExpression ()](#apidoc.element.regenerator.types.builders.newExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>newStatement ()](#apidoc.element.regenerator.types.builders.newStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>noop ()](#apidoc.element.regenerator.types.builders.noop)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>nullLiteral ()](#apidoc.element.regenerator.types.builders.nullLiteral)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>nullLiteralStatement ()](#apidoc.element.regenerator.types.builders.nullLiteralStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>nullLiteralTypeAnnotation ()](#apidoc.element.regenerator.types.builders.nullLiteralTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>nullTypeAnnotation ()](#apidoc.element.regenerator.types.builders.nullTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>nullableTypeAnnotation ()](#apidoc.element.regenerator.types.builders.nullableTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>numberLiteralTypeAnnotation ()](#apidoc.element.regenerator.types.builders.numberLiteralTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>numberTypeAnnotation ()](#apidoc.element.regenerator.types.builders.numberTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>numericLiteral ()](#apidoc.element.regenerator.types.builders.numericLiteral)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>numericLiteralStatement ()](#apidoc.element.regenerator.types.builders.numericLiteralStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>numericLiteralTypeAnnotation ()](#apidoc.element.regenerator.types.builders.numericLiteralTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectExpression ()](#apidoc.element.regenerator.types.builders.objectExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectMethod ()](#apidoc.element.regenerator.types.builders.objectMethod)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectPattern ()](#apidoc.element.regenerator.types.builders.objectPattern)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectProperty ()](#apidoc.element.regenerator.types.builders.objectProperty)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectStatement ()](#apidoc.element.regenerator.types.builders.objectStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectTypeAnnotation ()](#apidoc.element.regenerator.types.builders.objectTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectTypeCallProperty ()](#apidoc.element.regenerator.types.builders.objectTypeCallProperty)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectTypeIndexer ()](#apidoc.element.regenerator.types.builders.objectTypeIndexer)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectTypeProperty ()](#apidoc.element.regenerator.types.builders.objectTypeProperty)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>parenthesizedExpression ()](#apidoc.element.regenerator.types.builders.parenthesizedExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>parenthesizedStatement ()](#apidoc.element.regenerator.types.builders.parenthesizedStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>position ()](#apidoc.element.regenerator.types.builders.position)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>program ()](#apidoc.element.regenerator.types.builders.program)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>property ()](#apidoc.element.regenerator.types.builders.property)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>propertyPattern ()](#apidoc.element.regenerator.types.builders.propertyPattern)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>qualifiedTypeIdentifier ()](#apidoc.element.regenerator.types.builders.qualifiedTypeIdentifier)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>regExpLiteral ()](#apidoc.element.regenerator.types.builders.regExpLiteral)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>regExpLiteralStatement ()](#apidoc.element.regenerator.types.builders.regExpLiteralStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>restElement ()](#apidoc.element.regenerator.types.builders.restElement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>restProperty ()](#apidoc.element.regenerator.types.builders.restProperty)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>returnStatement ()](#apidoc.element.regenerator.types.builders.returnStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>sequenceExpression ()](#apidoc.element.regenerator.types.builders.sequenceExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>sequenceStatement ()](#apidoc.element.regenerator.types.builders.sequenceStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>sourceLocation ()](#apidoc.element.regenerator.types.builders.sourceLocation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>spreadElement ()](#apidoc.element.regenerator.types.builders.spreadElement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>spreadElementPattern ()](#apidoc.element.regenerator.types.builders.spreadElementPattern)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>spreadProperty ()](#apidoc.element.regenerator.types.builders.spreadProperty)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>spreadPropertyPattern ()](#apidoc.element.regenerator.types.builders.spreadPropertyPattern)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>stringLiteral ()](#apidoc.element.regenerator.types.builders.stringLiteral)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>stringLiteralStatement ()](#apidoc.element.regenerator.types.builders.stringLiteralStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>stringLiteralTypeAnnotation ()](#apidoc.element.regenerator.types.builders.stringLiteralTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>stringTypeAnnotation ()](#apidoc.element.regenerator.types.builders.stringTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>super ()](#apidoc.element.regenerator.types.builders.super)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>superStatement ()](#apidoc.element.regenerator.types.builders.superStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>switchCase ()](#apidoc.element.regenerator.types.builders.switchCase)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>switchStatement ()](#apidoc.element.regenerator.types.builders.switchStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>taggedTemplateExpression ()](#apidoc.element.regenerator.types.builders.taggedTemplateExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>taggedTemplateStatement ()](#apidoc.element.regenerator.types.builders.taggedTemplateStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>templateElement ()](#apidoc.element.regenerator.types.builders.templateElement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>templateLiteral ()](#apidoc.element.regenerator.types.builders.templateLiteral)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>templateLiteralStatement ()](#apidoc.element.regenerator.types.builders.templateLiteralStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>thisExpression ()](#apidoc.element.regenerator.types.builders.thisExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>thisStatement ()](#apidoc.element.regenerator.types.builders.thisStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>thisTypeAnnotation ()](#apidoc.element.regenerator.types.builders.thisTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>throwStatement ()](#apidoc.element.regenerator.types.builders.throwStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>tryStatement ()](#apidoc.element.regenerator.types.builders.tryStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>tupleTypeAnnotation ()](#apidoc.element.regenerator.types.builders.tupleTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeAlias ()](#apidoc.element.regenerator.types.builders.typeAlias)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeAnnotation ()](#apidoc.element.regenerator.types.builders.typeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeCastExpression ()](#apidoc.element.regenerator.types.builders.typeCastExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeCastStatement ()](#apidoc.element.regenerator.types.builders.typeCastStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeParameter ()](#apidoc.element.regenerator.types.builders.typeParameter)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeParameterDeclaration ()](#apidoc.element.regenerator.types.builders.typeParameterDeclaration)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeParameterInstantiation ()](#apidoc.element.regenerator.types.builders.typeParameterInstantiation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeofTypeAnnotation ()](#apidoc.element.regenerator.types.builders.typeofTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>unaryExpression ()](#apidoc.element.regenerator.types.builders.unaryExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>unaryStatement ()](#apidoc.element.regenerator.types.builders.unaryStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>unionTypeAnnotation ()](#apidoc.element.regenerator.types.builders.unionTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>updateExpression ()](#apidoc.element.regenerator.types.builders.updateExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>updateStatement ()](#apidoc.element.regenerator.types.builders.updateStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>variableDeclaration ()](#apidoc.element.regenerator.types.builders.variableDeclaration)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>variableDeclarator ()](#apidoc.element.regenerator.types.builders.variableDeclarator)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>voidTypeAnnotation ()](#apidoc.element.regenerator.types.builders.voidTypeAnnotation)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>whileStatement ()](#apidoc.element.regenerator.types.builders.whileStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>withStatement ()](#apidoc.element.regenerator.types.builders.withStatement)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>yieldExpression ()](#apidoc.element.regenerator.types.builders.yieldExpression)
1.  [function <span class="apidocSignatureSpan">regenerator.types.builders.</span>yieldStatement ()](#apidoc.element.regenerator.types.builders.yieldStatement)

#### [module regenerator.util](#apidoc.module.regenerator.util)
1.  [function <span class="apidocSignatureSpan">regenerator.util.</span>defaults (obj)](#apidoc.element.regenerator.util.defaults)
1.  [function <span class="apidocSignatureSpan">regenerator.util.</span>isReference (path, name)](#apidoc.element.regenerator.util.isReference)
1.  [function <span class="apidocSignatureSpan">regenerator.util.</span>runtimeProperty (name)](#apidoc.element.regenerator.util.runtimeProperty)

#### [module regenerator.visit](#apidoc.module.regenerator.visit)
1.  [function <span class="apidocSignatureSpan">regenerator.visit.</span>transform (node, options)](#apidoc.element.regenerator.visit.transform)



# <a name="apidoc.module.regenerator"></a>[module regenerator](#apidoc.module.regenerator)

#### <a name="apidoc.element.regenerator.compile"></a>[function <span class="apidocSignatureSpan">regenerator.</span>compile (source, options)](#apidoc.element.regenerator.compile)
- description and source-code
```javascript
function compile(source, options) {
  var result;

  options = utils.defaults(options || {}, {
    includeRuntime: false
  });

  // Shortcut: Transform only if generators or async functions present.
  if (genOrAsyncFunExp.test(source)) {
    result = require("babel-core").transform(source, transformOptions);
  } else {
    result = { code: source };
  }

  if (options.includeRuntime === true) {
    result.code = getRuntimeCode() + "\n" + result.code;
  }

  return result;
}
```
- example usage
```shell
...
regenerator es6.js > es5.js # Just the transform.
regenerator --include-runtime es6.js > es5.js # Add the runtime too.
regenerator src lib # Transform every .js file in src and output to lib.
'''

Programmatic usage:
'''js
var es5Source = require("regenerator").compile(es6Source).code;
var es5SourceWithRuntime = require("regenerator").compile(es6Source, {
  includeRuntime: true
}).code;
'''

AST transformation:
'''js
...
```

#### <a name="apidoc.element.regenerator.runtime"></a>[function <span class="apidocSignatureSpan">regenerator.</span>runtime ()](#apidoc.element.regenerator.runtime)
- description and source-code
```javascript
function runtime() {
  regeneratorRuntime = require("regenerator-runtime");
}
```
- example usage
```shell
...
}

// To get a writable stream for use as a browserify transform, call
// require("regenerator")().
module.exports = exports;

// To include the runtime globally in the current node process, call
// require("regenerator").runtime().
function runtime() {
  regeneratorRuntime = require("regenerator-runtime");
}
exports.runtime = runtime;
runtime.path = require("regenerator-runtime/path.js").path;

var cachedRuntimeCode;
...
```

#### <a name="apidoc.element.regenerator.transform"></a>[function <span class="apidocSignatureSpan">regenerator.</span>transform (node, options)](#apidoc.element.regenerator.transform)
- description and source-code
```javascript
function transform(node, options) {
  options = util.defaults(options || {}, {
    includeRuntime: false
  });

  var result = require("babel-core").transformFromAst(node, null, {
    presets: [require("regenerator-preset")],
    code: false,
    ast: true
  });

  node = result.ast;

  if (options.includeRuntime === true) {
    injectRuntime(n.File.check(node) ? node.program : node);
  }

  return node;
}
```
- example usage
```shell
...
}).code;
'''

AST transformation:
'''js
var recast = require("recast");
var ast = recast.parse(es6Source);
ast = require("regenerator").transform(ast);
var es5Source = recast.print(ast);
'''

How can you get involved?
---

The easiest way to get involved is to look for buggy examples using [the
...
```

#### <a name="apidoc.element.regenerator.types.NodePath"></a>[function <span class="apidocSignatureSpan">regenerator.</span>types.NodePath (value, parentPath, name)](#apidoc.element.regenerator.types.NodePath)
- description and source-code
```javascript
function NodePath(value, parentPath, name) {
    if (!(this instanceof NodePath)) {
        throw new Error("NodePath constructor cannot be invoked without 'new'");
    }
    Path.call(this, value, parentPath, name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Path"></a>[function <span class="apidocSignatureSpan">regenerator.</span>types.Path (value, parentPath, name)](#apidoc.element.regenerator.types.Path)
- description and source-code
```javascript
function Path(value, parentPath, name) {
    if (!(this instanceof Path)) {
        throw new Error("Path constructor cannot be invoked without 'new'");
    }

    if (parentPath) {
        if (!(parentPath instanceof Path)) {
            throw new Error("");
        }
    } else {
        parentPath = null;
        name = null;
    }

    // The value encapsulated by this Path, generally equal to
    // parentPath.value[name] if we have a parentPath.
    this.value = value;

    // The immediate parent Path of this Path.
    this.parentPath = parentPath;

    // The name of the property of parentPath.value through which this
    // Path's value was reached.
    this.name = name;

    // Calling path.get("child") multiple times always returns the same
    // child Path object, for both performance and consistency reasons.
    this.__childCache = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.PathVisitor"></a>[function <span class="apidocSignatureSpan">regenerator.</span>types.PathVisitor ()](#apidoc.element.regenerator.types.PathVisitor)
- description and source-code
```javascript
function PathVisitor() {
    if (!(this instanceof PathVisitor)) {
        throw new Error(
          "PathVisitor constructor cannot be invoked without 'new'"
        );
    }

    // Permanent state.
    this._reusableContextStack = [];

    this._methodNameTable = computeMethodNameTable(this);
    this._shouldVisitComments =
      hasOwn.call(this._methodNameTable, "Block") ||
      hasOwn.call(this._methodNameTable, "Line");

    this.Context = makeContextConstructor(this);

    // State reset every time PathVisitor.prototype.visit is called.
    this._visiting = false;
    this._changeReported = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Type"></a>[function <span class="apidocSignatureSpan">regenerator.</span>types.Type (check, name)](#apidoc.element.regenerator.types.Type)
- description and source-code
```javascript
function Type(check, name) {
    var self = this;
    if (!(self instanceof Type)) {
        throw new Error("Type constructor cannot be invoked without 'new'");
    }

    // Unfortunately we can't elegantly reuse isFunction and isString,
    // here, because this code is executed while defining those types.
    if (objToStr.call(check) !== funObjStr) {
        throw new Error(check + " is not a function");
    }

    // The 'name' parameter can be either a function or a string.
    var nameObjStr = objToStr.call(name);
    if (!(nameObjStr === funObjStr ||
      nameObjStr === strObjStr)) {
        throw new Error(name + " is neither a function nor a string");
    }

    Object.defineProperties(self, {
        name: {value: name},
        check: {
            value: function (value, deep) {
                var result = check.call(self, value, deep);
                if (!result && deep && objToStr.call(deep) === funObjStr)
                    deep(self, value);
                return result;
            }
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.astNodesAreEquivalent"></a>[function <span class="apidocSignatureSpan">regenerator.</span>types.astNodesAreEquivalent (a, b, problemPath)](#apidoc.element.regenerator.types.astNodesAreEquivalent)
- description and source-code
```javascript
function astNodesAreEquivalent(a, b, problemPath) {
    if (isArray.check(problemPath)) {
        problemPath.length = 0;
    } else {
        problemPath = null;
    }

    return areEquivalent(a, b, problemPath);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.regenerator.runtime_module"></a>[module regenerator.runtime_module](#apidoc.module.regenerator.runtime_module)

#### <a name="apidoc.element.regenerator.runtime_module.AsyncIterator"></a>[function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>AsyncIterator (generator)](#apidoc.element.regenerator.runtime_module.AsyncIterator)
- description and source-code
```javascript
function AsyncIterator(generator) {
  function invoke(method, arg, resolve, reject) {
    var record = tryCatch(generator[method], generator, arg);
    if (record.type === "throw") {
      reject(record.arg);
    } else {
      var result = record.arg;
      var value = result.value;
      if (value &&
          typeof value === "object" &&
          hasOwn.call(value, "__await")) {
        return Promise.resolve(value.__await).then(function(value) {
          invoke("next", value, resolve, reject);
        }, function(err) {
          invoke("throw", err, resolve, reject);
        });
      }

      return Promise.resolve(value).then(function(unwrapped) {
        // When a yielded Promise is resolved, its final value becomes
        // the .value of the Promise<{value,done}> result for the
        // current iteration. If the Promise is rejected, however, the
        // result for this iteration will be rejected with the same
        // reason. Note that rejections of yielded Promises are not
        // thrown back into the generator function, as is the case
        // when an awaited Promise is rejected. This difference in
        // behavior between yield and await is important, because it
        // allows the consumer to decide what to do with the yielded
        // rejection (swallow it and continue, manually .throw it back
        // into the generator, abandon iteration, whatever). With
        // await, by contrast, there is no opportunity to examine the
        // rejection reason outside the generator function, so the
        // only option is to throw it from the await expression, and
        // let the generator function handle the exception.
        result.value = unwrapped;
        resolve(result);
      }, reject);
    }
  }

  if (typeof process === "object" && process.domain) {
    invoke = process.domain.bind(invoke);
  }

  var previousPromise;

  function enqueue(method, arg) {
    function callInvokeWithMethodAndArg() {
      return new Promise(function(resolve, reject) {
        invoke(method, arg, resolve, reject);
      });
    }

    return previousPromise =
      // If enqueue has been called before, then we want to wait until
      // all previous Promises have been resolved before calling invoke,
      // so that results are always delivered in the correct order. If
      // enqueue has not been called before, then it is important to
      // call invoke immediately, without waiting on a callback to fire,
      // so that the async generator function has the opportunity to do
      // any necessary setup in a predictable way. This predictability
      // is why the Promise constructor synchronously invokes its
      // executor callback, and why async functions synchronously
      // execute code before the first await. Since we implement simple
      // async functions in terms of async generators, it is especially
      // important to get this right, even though it requires care.
      previousPromise ? previousPromise.then(
        callInvokeWithMethodAndArg,
        // Avoid propagating failures to Promises returned by later
        // invocations of the iterator.
        callInvokeWithMethodAndArg
      ) : callInvokeWithMethodAndArg();
  }

  // Define the unified helper method that is used to implement .next,
  // .throw, and .return (see defineIteratorMethods).
  this._invoke = enqueue;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.runtime_module.async"></a>[function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>async (innerFn, outerFn, self, tryLocsList)](#apidoc.element.regenerator.runtime_module.async)
- description and source-code
```javascript
async = function (innerFn, outerFn, self, tryLocsList) {
  var iter = new AsyncIterator(
    wrap(innerFn, outerFn, self, tryLocsList)
  );

  return runtime.isGeneratorFunction(outerFn)
    ? iter // If outerFn is a generator, return the full iterator.
    : iter.next().then(function(result) {
        return result.done ? result.value : iter.next();
      });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.runtime_module.awrap"></a>[function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>awrap (arg)](#apidoc.element.regenerator.runtime_module.awrap)
- description and source-code
```javascript
awrap = function (arg) {
  return { __await: arg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.runtime_module.isGeneratorFunction"></a>[function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>isGeneratorFunction (genFun)](#apidoc.element.regenerator.runtime_module.isGeneratorFunction)
- description and source-code
```javascript
isGeneratorFunction = function (genFun) {
  var ctor = typeof genFun === "function" && genFun.constructor;
  return ctor
    ? ctor === GeneratorFunction ||
      // For the native GeneratorFunction constructor, the best we can
      // do is to check its .name property.
      (ctor.displayName || ctor.name) === "GeneratorFunction"
    : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.runtime_module.keys"></a>[function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>keys (object)](#apidoc.element.regenerator.runtime_module.keys)
- description and source-code
```javascript
keys = function (object) {
  var keys = [];
  for (var key in object) {
    keys.push(key);
  }
  keys.reverse();

  // Rather than returning an object with a next method, we keep
  // things simple and return the next function itself.
  return function next() {
    while (keys.length) {
      var key = keys.pop();
      if (key in object) {
        next.value = key;
        next.done = false;
        return next;
      }
    }

    // To avoid creating an additional object, we just hang the .value
    // and .done properties off the next function object itself. This
    // also ensures that the minifier will not anonymize the function.
    next.done = true;
    return next;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.runtime_module.mark"></a>[function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>mark (genFun)](#apidoc.element.regenerator.runtime_module.mark)
- description and source-code
```javascript
mark = function (genFun) {
  if (Object.setPrototypeOf) {
    Object.setPrototypeOf(genFun, GeneratorFunctionPrototype);
  } else {
    genFun.__proto__ = GeneratorFunctionPrototype;
    if (!(toStringTagSymbol in genFun)) {
      genFun[toStringTagSymbol] = "GeneratorFunction";
    }
  }
  genFun.prototype = Object.create(Gp);
  return genFun;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.runtime_module.values"></a>[function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>values (iterable)](#apidoc.element.regenerator.runtime_module.values)
- description and source-code
```javascript
function values(iterable) {
  if (iterable) {
    var iteratorMethod = iterable[iteratorSymbol];
    if (iteratorMethod) {
      return iteratorMethod.call(iterable);
    }

    if (typeof iterable.next === "function") {
      return iterable;
    }

    if (!isNaN(iterable.length)) {
      var i = -1, next = function next() {
        while (++i < iterable.length) {
          if (hasOwn.call(iterable, i)) {
            next.value = iterable[i];
            next.done = false;
            return next;
          }
        }

        next.value = undefined;
        next.done = true;

        return next;
      };

      return next.next = next;
    }
  }

  // Return an iterator with no values.
  return { next: doneResult };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.runtime_module.wrap"></a>[function <span class="apidocSignatureSpan">regenerator.runtime_module.</span>wrap (innerFn, outerFn, self, tryLocsList)](#apidoc.element.regenerator.runtime_module.wrap)
- description and source-code
```javascript
function wrap(innerFn, outerFn, self, tryLocsList) {
  // If outerFn provided and outerFn.prototype is a Generator, then outerFn.prototype instanceof Generator.
  var protoGenerator = outerFn && outerFn.prototype instanceof Generator ? outerFn : Generator;
  var generator = Object.create(protoGenerator.prototype);
  var context = new Context(tryLocsList || []);

  // The ._invoke method unifies the implementations of the .next,
  // .throw, and .return methods.
  generator._invoke = makeInvokeMethod(innerFn, self, context);

  return generator;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.regenerator.types"></a>[module regenerator.types](#apidoc.module.regenerator.types)

#### <a name="apidoc.element.regenerator.types.NodePath"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>NodePath (value, parentPath, name)](#apidoc.element.regenerator.types.NodePath)
- description and source-code
```javascript
function NodePath(value, parentPath, name) {
    if (!(this instanceof NodePath)) {
        throw new Error("NodePath constructor cannot be invoked without 'new'");
    }
    Path.call(this, value, parentPath, name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Path"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>Path (value, parentPath, name)](#apidoc.element.regenerator.types.Path)
- description and source-code
```javascript
function Path(value, parentPath, name) {
    if (!(this instanceof Path)) {
        throw new Error("Path constructor cannot be invoked without 'new'");
    }

    if (parentPath) {
        if (!(parentPath instanceof Path)) {
            throw new Error("");
        }
    } else {
        parentPath = null;
        name = null;
    }

    // The value encapsulated by this Path, generally equal to
    // parentPath.value[name] if we have a parentPath.
    this.value = value;

    // The immediate parent Path of this Path.
    this.parentPath = parentPath;

    // The name of the property of parentPath.value through which this
    // Path's value was reached.
    this.name = name;

    // Calling path.get("child") multiple times always returns the same
    // child Path object, for both performance and consistency reasons.
    this.__childCache = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.PathVisitor"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>PathVisitor ()](#apidoc.element.regenerator.types.PathVisitor)
- description and source-code
```javascript
function PathVisitor() {
    if (!(this instanceof PathVisitor)) {
        throw new Error(
          "PathVisitor constructor cannot be invoked without 'new'"
        );
    }

    // Permanent state.
    this._reusableContextStack = [];

    this._methodNameTable = computeMethodNameTable(this);
    this._shouldVisitComments =
      hasOwn.call(this._methodNameTable, "Block") ||
      hasOwn.call(this._methodNameTable, "Line");

    this.Context = makeContextConstructor(this);

    // State reset every time PathVisitor.prototype.visit is called.
    this._visiting = false;
    this._changeReported = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Type"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>Type (check, name)](#apidoc.element.regenerator.types.Type)
- description and source-code
```javascript
function Type(check, name) {
    var self = this;
    if (!(self instanceof Type)) {
        throw new Error("Type constructor cannot be invoked without 'new'");
    }

    // Unfortunately we can't elegantly reuse isFunction and isString,
    // here, because this code is executed while defining those types.
    if (objToStr.call(check) !== funObjStr) {
        throw new Error(check + " is not a function");
    }

    // The 'name' parameter can be either a function or a string.
    var nameObjStr = objToStr.call(name);
    if (!(nameObjStr === funObjStr ||
      nameObjStr === strObjStr)) {
        throw new Error(name + " is neither a function nor a string");
    }

    Object.defineProperties(self, {
        name: {value: name},
        check: {
            value: function (value, deep) {
                var result = check.call(self, value, deep);
                if (!result && deep && objToStr.call(deep) === funObjStr)
                    deep(self, value);
                return result;
            }
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.astNodesAreEquivalent"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>astNodesAreEquivalent (a, b, problemPath)](#apidoc.element.regenerator.types.astNodesAreEquivalent)
- description and source-code
```javascript
function astNodesAreEquivalent(a, b, problemPath) {
    if (isArray.check(problemPath)) {
        problemPath.length = 0;
    } else {
        problemPath = null;
    }

    return areEquivalent(a, b, problemPath);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.defineMethod"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>defineMethod (name, func)](#apidoc.element.regenerator.types.defineMethod)
- description and source-code
```javascript
defineMethod = function (name, func) {
    var old = nodePrototype[name];

    // Pass undefined as func to delete nodePrototype[name].
    if (isUndefined.check(func)) {
        delete nodePrototype[name];

    } else {
        isFunction.assert(func);

        Object.defineProperty(nodePrototype, name, {
            enumerable: true, // For discoverability.
            configurable: true, // For delete proto[name].
            value: func
        });
    }

    return old;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.eachField"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>eachField (object, callback, context)](#apidoc.element.regenerator.types.eachField)
- description and source-code
```javascript
eachField = function (object, callback, context) {
    getFieldNames(object).forEach(function (name) {
        callback.call(this, name, getFieldValue(object, name));
    }, context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.finalize"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>finalize ()](#apidoc.element.regenerator.types.finalize)
- description and source-code
```javascript
finalize = function () {
    Object.keys(defCache).forEach(function (name) {
        defCache[name].finalize();
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.getFieldNames"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>getFieldNames (object)](#apidoc.element.regenerator.types.getFieldNames)
- description and source-code
```javascript
function getFieldNames(object) {
    var d = Def.fromValue(object);
    if (d) {
        return d.fieldNames.slice(0);
    }

    if ("type" in object) {
        throw new Error(
          "did not recognize object of type " +
          JSON.stringify(object.type)
        );
    }

    return Object.keys(object);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.getFieldValue"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>getFieldValue (object, fieldName)](#apidoc.element.regenerator.types.getFieldValue)
- description and source-code
```javascript
function getFieldValue(object, fieldName) {
    var d = Def.fromValue(object);
    if (d) {
        var field = d.allFields[fieldName];
        if (field) {
            return field.getValue(object);
        }
    }

    return object && object[fieldName];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.getSupertypeNames"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>getSupertypeNames (typeName)](#apidoc.element.regenerator.types.getSupertypeNames)
- description and source-code
```javascript
getSupertypeNames = function (typeName) {
    if (!hasOwn.call(defCache, typeName)) {
        throw new Error("");
    }
    var d = defCache[typeName];
    if (d.finalized !== true) {
        throw new Error("");
    }
    return d.supertypeList.slice(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.someField"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>someField (object, callback, context)](#apidoc.element.regenerator.types.someField)
- description and source-code
```javascript
someField = function (object, callback, context) {
    return getFieldNames(object).some(function (name) {
        return callback.call(this, name, getFieldValue(object, name));
    }, context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.use"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>use (plugin)](#apidoc.element.regenerator.types.use)
- description and source-code
```javascript
function use(plugin) {
    var idx = used.indexOf(plugin);
    if (idx === -1) {
        idx = used.length;
        used.push(plugin);
        usedResult[idx] = plugin(fork);
    }
    return usedResult[idx];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.visit"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>visit (node, methods)](#apidoc.element.regenerator.types.visit)
- description and source-code
```javascript
function visit(node, methods) {
    return PathVisitor.fromMethodsObject(methods).visit(node);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.regenerator.types.NodePath"></a>[module regenerator.types.NodePath](#apidoc.module.regenerator.types.NodePath)

#### <a name="apidoc.element.regenerator.types.NodePath.NodePath"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>NodePath (value, parentPath, name)](#apidoc.element.regenerator.types.NodePath.NodePath)
- description and source-code
```javascript
function NodePath(value, parentPath, name) {
    if (!(this instanceof NodePath)) {
        throw new Error("NodePath constructor cannot be invoked without 'new'");
    }
    Path.call(this, value, parentPath, name);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.regenerator.types.NodePath.prototype"></a>[module regenerator.types.NodePath.prototype](#apidoc.module.regenerator.types.NodePath.prototype)

#### <a name="apidoc.element.regenerator.types.NodePath.prototype._computeNode"></a>[function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>_computeNode ()](#apidoc.element.regenerator.types.NodePath.prototype._computeNode)
- description and source-code
```javascript
_computeNode = function () {
    var value = this.value;
    if (n.Node.check(value)) {
        return value;
    }

    var pp = this.parentPath;
    return pp && pp.node || null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.NodePath.prototype._computeParent"></a>[function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>_computeParent ()](#apidoc.element.regenerator.types.NodePath.prototype._computeParent)
- description and source-code
```javascript
_computeParent = function () {
    var value = this.value;
    var pp = this.parentPath;

    if (!n.Node.check(value)) {
        while (pp && !n.Node.check(pp.value)) {
            pp = pp.parentPath;
        }

        if (pp) {
            pp = pp.parentPath;
        }
    }

    while (pp && !n.Node.check(pp.value)) {
        pp = pp.parentPath;
    }

    return pp || null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.NodePath.prototype._computeScope"></a>[function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>_computeScope ()](#apidoc.element.regenerator.types.NodePath.prototype._computeScope)
- description and source-code
```javascript
_computeScope = function () {
    var value = this.value;
    var pp = this.parentPath;
    var scope = pp && pp.scope;

    if (n.Node.check(value) &&
      Scope.isEstablishedBy(value)) {
        scope = new Scope(this, scope);
    }

    return scope || null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.NodePath.prototype.canBeFirstInStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>canBeFirstInStatement ()](#apidoc.element.regenerator.types.NodePath.prototype.canBeFirstInStatement)
- description and source-code
```javascript
canBeFirstInStatement = function () {
    var node = this.node;
    return !n.FunctionExpression.check(node)
      && !n.ObjectExpression.check(node);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.NodePath.prototype.firstInStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>firstInStatement ()](#apidoc.element.regenerator.types.NodePath.prototype.firstInStatement)
- description and source-code
```javascript
firstInStatement = function () {
    return firstInStatement(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.NodePath.prototype.getValueProperty"></a>[function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>getValueProperty (name)](#apidoc.element.regenerator.types.NodePath.prototype.getValueProperty)
- description and source-code
```javascript
getValueProperty = function (name) {
    return types.getFieldValue(this.value, name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.NodePath.prototype.needsParens"></a>[function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>needsParens (assumeExpressionContext)](#apidoc.element.regenerator.types.NodePath.prototype.needsParens)
- description and source-code
```javascript
needsParens = function (assumeExpressionContext) {
    var pp = this.parentPath;
    if (!pp) {
        return false;
    }

    var node = this.value;

    // Only expressions need parentheses.
    if (!n.Expression.check(node)) {
        return false;
    }

    // Identifiers never need parentheses.
    if (node.type === "Identifier") {
        return false;
    }

    while (!n.Node.check(pp.value)) {
        pp = pp.parentPath;
        if (!pp) {
            return false;
        }
    }

    var parent = pp.value;

    switch (node.type) {
        case "UnaryExpression":
        case "SpreadElement":
        case "SpreadProperty":
            return parent.type === "MemberExpression"
              && this.name === "object"
              && parent.object === node;

        case "BinaryExpression":
        case "LogicalExpression":
            switch (parent.type) {
                case "CallExpression":
                    return this.name === "callee"
                      && parent.callee === node;

                case "UnaryExpression":
                case "SpreadElement":
                case "SpreadProperty":
                    return true;

                case "MemberExpression":
                    return this.name === "object"
                      && parent.object === node;

                case "BinaryExpression":
                case "LogicalExpression":
                    var po = parent.operator;
                    var pp = PRECEDENCE[po];
                    var no = node.operator;
                    var np = PRECEDENCE[no];

                    if (pp > np) {
                        return true;
                    }

                    if (pp === np && this.name === "right") {
                        if (parent.right !== node) {
                            throw new Error("Nodes must be equal");
                        }
                        return true;
                    }

                default:
                    return false;
            }

        case "SequenceExpression":
            switch (parent.type) {
                case "ForStatement":
                    // Although parentheses wouldn't hurt around sequence
                    // expressions in the head of for loops, traditional style
                    // dictates that e.g. i++, j++ should not be wrapped with
                    // parentheses.
                    return false;

                case "ExpressionStatement":
                    return this.name !== "expression";

                default:
                    // Otherwise err on the side of overparenthesization, adding
                    // explicit exceptions above if this proves overzealous.
                    return true;
            }

        case "YieldExpression":
            switch (parent.type) {
                case "BinaryExpression":
                case "LogicalExpression":
                case "UnaryExpression":
                case "SpreadElement":
                case "SpreadProperty":
                case "CallExpression":
                case "MemberExpression":
                case "NewExpression":
                case "ConditionalExpression":
                case "YieldExpression":
                    return true;

                default:
                    return false;
            }

        case "Literal":
            return parent.type === "MemberExpression"
              && isNumber.check(node.value)
              && this.name === "object"
              && parent.object === node;

        case "AssignmentExpression":
        case "ConditionalExpression":
            switch (parent.type) {
                case "UnaryExpression":
                case "SpreadElement":
                case "SpreadProperty":
                case "BinaryExpression":
                case "LogicalExpression":
                    return true;

                case "CallExpression":
                    return this.name === "callee"
                      && parent.callee === node;

                case "ConditionalExpression":
                    return this.name === " ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.NodePath.prototype.prune"></a>[function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>prune ()](#apidoc.element.regenerator.types.NodePath.prototype.prune)
- description and source-code
```javascript
prune = function () {
    var remainingNodePath = this.parent;

    this.replace();

    return cleanUpNodesAfterPrune(remainingNodePath);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.NodePath.prototype.replace"></a>[function <span class="apidocSignatureSpan">regenerator.types.NodePath.prototype.</span>replace ()](#apidoc.element.regenerator.types.NodePath.prototype.replace)
- description and source-code
```javascript
replace = function () {
    delete this.node;
    delete this.parent;
    delete this.scope;
    return Path.prototype.replace.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.regenerator.types.Path"></a>[module regenerator.types.Path](#apidoc.module.regenerator.types.Path)

#### <a name="apidoc.element.regenerator.types.Path.Path"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>Path (value, parentPath, name)](#apidoc.element.regenerator.types.Path.Path)
- description and source-code
```javascript
function Path(value, parentPath, name) {
    if (!(this instanceof Path)) {
        throw new Error("Path constructor cannot be invoked without 'new'");
    }

    if (parentPath) {
        if (!(parentPath instanceof Path)) {
            throw new Error("");
        }
    } else {
        parentPath = null;
        name = null;
    }

    // The value encapsulated by this Path, generally equal to
    // parentPath.value[name] if we have a parentPath.
    this.value = value;

    // The immediate parent Path of this Path.
    this.parentPath = parentPath;

    // The name of the property of parentPath.value through which this
    // Path's value was reached.
    this.name = name;

    // Calling path.get("child") multiple times always returns the same
    // child Path object, for both performance and consistency reasons.
    this.__childCache = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.regenerator.types.Path.prototype"></a>[module regenerator.types.Path.prototype](#apidoc.module.regenerator.types.Path.prototype)

#### <a name="apidoc.element.regenerator.types.Path.prototype.each"></a>[function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>each (callback, context)](#apidoc.element.regenerator.types.Path.prototype.each)
- description and source-code
```javascript
function each(callback, context) {
    var childPaths = [];
    var len = this.value.length;
    var i = 0;

    // Collect all the original child paths before invoking the callback.
    for (var i = 0; i < len; ++i) {
        if (hasOwn.call(this.value, i)) {
            childPaths[i] = this.get(i);
        }
    }

    // Invoke the callback on just the original child paths, regardless of
    // any modifications made to the array by the callback. I chose these
    // semantics over cleverly invoking the callback on new elements because
    // this way is much easier to reason about.
    context = context || this;
    for (i = 0; i < len; ++i) {
        if (hasOwn.call(childPaths, i)) {
            callback.call(context, childPaths[i]);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Path.prototype.filter"></a>[function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>filter (callback, context)](#apidoc.element.regenerator.types.Path.prototype.filter)
- description and source-code
```javascript
function filter(callback, context) {
    var result = [];

    this.each(function (childPath) {
        if (callback.call(this, childPath)) {
            result.push(childPath);
        }
    }, context);

    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Path.prototype.get"></a>[function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>get (name)](#apidoc.element.regenerator.types.Path.prototype.get)
- description and source-code
```javascript
function get(name) {
    var path = this;
    var names = arguments;
    var count = names.length;

    for (var i = 0; i < count; ++i) {
        path = getChildPath(path, names[i]);
    }

    return path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Path.prototype.getValueProperty"></a>[function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>getValueProperty (name)](#apidoc.element.regenerator.types.Path.prototype.getValueProperty)
- description and source-code
```javascript
function getValueProperty(name) {
    return this.value[name];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Path.prototype.insertAfter"></a>[function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>insertAfter (node)](#apidoc.element.regenerator.types.Path.prototype.insertAfter)
- description and source-code
```javascript
function insertAfter(node) {
    var pp = this.parentPath;
    var argc = arguments.length;
    var insertAtArgs = [this.name + 1];
    for (var i = 0; i < argc; ++i) {
        insertAtArgs.push(arguments[i]);
    }
    return pp.insertAt.apply(pp, insertAtArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Path.prototype.insertAt"></a>[function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>insertAt (index, node)](#apidoc.element.regenerator.types.Path.prototype.insertAt)
- description and source-code
```javascript
function insertAt(index, node) {
    var argc = arguments.length;
    var move = getMoves(this, argc - 1, index);
    if (move === emptyMoves) {
        return this;
    }

    index = Math.max(index, 0);

    for (var i = 1; i < argc; ++i) {
        this.value[index + i - 1] = arguments[i];
    }

    move();

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Path.prototype.insertBefore"></a>[function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>insertBefore (node)](#apidoc.element.regenerator.types.Path.prototype.insertBefore)
- description and source-code
```javascript
function insertBefore(node) {
    var pp = this.parentPath;
    var argc = arguments.length;
    var insertAtArgs = [this.name];
    for (var i = 0; i < argc; ++i) {
        insertAtArgs.push(arguments[i]);
    }
    return pp.insertAt.apply(pp, insertAtArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Path.prototype.map"></a>[function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>map (callback, context)](#apidoc.element.regenerator.types.Path.prototype.map)
- description and source-code
```javascript
function map(callback, context) {
    var result = [];

    this.each(function (childPath) {
        result.push(callback.call(this, childPath));
    }, context);

    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Path.prototype.pop"></a>[function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>pop ()](#apidoc.element.regenerator.types.Path.prototype.pop)
- description and source-code
```javascript
function pop() {
    isArray.assert(this.value);
    var cache = getChildCache(this);
    delete cache[this.value.length - 1];
    delete cache.length;
    return this.value.pop();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Path.prototype.push"></a>[function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>push (node)](#apidoc.element.regenerator.types.Path.prototype.push)
- description and source-code
```javascript
function push(node) {
    isArray.assert(this.value);
    delete getChildCache(this).length
    return this.value.push.apply(this.value, arguments);
}
```
- example usage
```shell
...
var genOrAsyncFunExp = /\bfunction\s*\*|\basync\b/;

function exports(file, options) {
var data = [];
return through(write, end);

function write(buf) {
  data.push(buf);
}

function end() {
  try {
    this.queue(compile(data.join(""), options).code);
    this.queue(null);
  } catch (e) { this.emit('error', e); }
...
```

#### <a name="apidoc.element.regenerator.types.Path.prototype.replace"></a>[function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>replace (replacement)](#apidoc.element.regenerator.types.Path.prototype.replace)
- description and source-code
```javascript
function replace(replacement) {
    var results = [];
    var parentValue = this.parentPath.value;
    var parentCache = getChildCache(this.parentPath);
    var count = arguments.length;

    repairRelationshipWithParent(this);

    if (isArray.check(parentValue)) {
        var originalLength = parentValue.length;
        var move = getMoves(this.parentPath, count - 1, this.name + 1);

        var spliceArgs = [this.name, 1];
        for (var i = 0; i < count; ++i) {
            spliceArgs.push(arguments[i]);
        }

        var splicedOut = parentValue.splice.apply(parentValue, spliceArgs);

        if (splicedOut[0] !== this.value) {
            throw new Error("");
        }
        if (parentValue.length !== (originalLength - 1 + count)) {
            throw new Error("");
        }

        move();

        if (count === 0) {
            delete this.value;
            delete parentCache[this.name];
            this.__childCache = null;

        } else {
            if (parentValue[this.name] !== replacement) {
                throw new Error("");
            }

            if (this.value !== replacement) {
                this.value = replacement;
                this.__childCache = null;
            }

            for (i = 0; i < count; ++i) {
                results.push(this.parentPath.get(this.name + i));
            }

            if (results[0] !== this) {
                throw new Error("");
            }
        }

    } else if (count === 1) {
        if (this.value !== replacement) {
            this.__childCache = null;
        }
        this.value = parentValue[this.name] = replacement;
        results.push(this);

    } else if (count === 0) {
        delete parentValue[this.name];
        delete this.value;
        this.__childCache = null;

        // Leave this path cached as parentCache[this.name], even though
        // it no longer has a value defined.

    } else {
        throw new Error("Could not replace path");
    }

    return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Path.prototype.shift"></a>[function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>shift ()](#apidoc.element.regenerator.types.Path.prototype.shift)
- description and source-code
```javascript
function shift() {
    var move = getMoves(this, -1);
    var result = this.value.shift();
    move();
    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Path.prototype.unshift"></a>[function <span class="apidocSignatureSpan">regenerator.types.Path.prototype.</span>unshift (node)](#apidoc.element.regenerator.types.Path.prototype.unshift)
- description and source-code
```javascript
function unshift(node) {
    var move = getMoves(this, arguments.length);
    var result = this.value.unshift.apply(this.value, arguments);
    move();
    return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.regenerator.types.PathVisitor"></a>[module regenerator.types.PathVisitor](#apidoc.module.regenerator.types.PathVisitor)

#### <a name="apidoc.element.regenerator.types.PathVisitor.PathVisitor"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>PathVisitor ()](#apidoc.element.regenerator.types.PathVisitor.PathVisitor)
- description and source-code
```javascript
function PathVisitor() {
    if (!(this instanceof PathVisitor)) {
        throw new Error(
          "PathVisitor constructor cannot be invoked without 'new'"
        );
    }

    // Permanent state.
    this._reusableContextStack = [];

    this._methodNameTable = computeMethodNameTable(this);
    this._shouldVisitComments =
      hasOwn.call(this._methodNameTable, "Block") ||
      hasOwn.call(this._methodNameTable, "Line");

    this.Context = makeContextConstructor(this);

    // State reset every time PathVisitor.prototype.visit is called.
    this._visiting = false;
    this._changeReported = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.PathVisitor.fromMethodsObject"></a>[function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.</span>fromMethodsObject (methods)](#apidoc.element.regenerator.types.PathVisitor.fromMethodsObject)
- description and source-code
```javascript
function fromMethodsObject(methods) {
    if (methods instanceof PathVisitor) {
        return methods;
    }

    if (!isObject.check(methods)) {
        // An empty visitor?
        return new PathVisitor;
    }

    function Visitor() {
        if (!(this instanceof Visitor)) {
            throw new Error(
              "Visitor constructor cannot be invoked without 'new'"
            );
        }
        PathVisitor.call(this);
    }

    var Vp = Visitor.prototype = Object.create(PVp);
    Vp.constructor = Visitor;

    extend(Vp, methods);
    extend(Visitor, PathVisitor);

    isFunction.assert(Visitor.fromMethodsObject);
    isFunction.assert(Visitor.visit);

    return new Visitor;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.PathVisitor.visit"></a>[function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.</span>visit (node, methods)](#apidoc.element.regenerator.types.PathVisitor.visit)
- description and source-code
```javascript
function visit(node, methods) {
    return PathVisitor.fromMethodsObject(methods).visit(node);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.regenerator.types.PathVisitor.prototype"></a>[module regenerator.types.PathVisitor.prototype](#apidoc.module.regenerator.types.PathVisitor.prototype)

#### <a name="apidoc.element.regenerator.types.PathVisitor.prototype.AbortRequest"></a>[function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>AbortRequest ()](#apidoc.element.regenerator.types.PathVisitor.prototype.AbortRequest)
- description and source-code
```javascript
function AbortRequest() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.PathVisitor.prototype.abort"></a>[function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>abort ()](#apidoc.element.regenerator.types.PathVisitor.prototype.abort)
- description and source-code
```javascript
abort = function () {
    var visitor = this;
    visitor._abortRequested = true;
    var request = new visitor.AbortRequest();

    // If you decide to catch this exception and stop it from propagating,
    // make sure to call its cancel method to avoid silencing other
    // exceptions that might be thrown later in the traversal.
    request.cancel = function () {
        visitor._abortRequested = false;
    };

    throw request;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.PathVisitor.prototype.acquireContext"></a>[function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>acquireContext (path)](#apidoc.element.regenerator.types.PathVisitor.prototype.acquireContext)
- description and source-code
```javascript
acquireContext = function (path) {
    if (this._reusableContextStack.length === 0) {
        return new this.Context(path);
    }
    return this._reusableContextStack.pop().reset(path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.PathVisitor.prototype.releaseContext"></a>[function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>releaseContext (context)](#apidoc.element.regenerator.types.PathVisitor.prototype.releaseContext)
- description and source-code
```javascript
releaseContext = function (context) {
    if (!(context instanceof this.Context)) {
        throw new Error("");
    }
    this._reusableContextStack.push(context);
    context.currentPath = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.PathVisitor.prototype.reportChanged"></a>[function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>reportChanged ()](#apidoc.element.regenerator.types.PathVisitor.prototype.reportChanged)
- description and source-code
```javascript
reportChanged = function () {
    this._changeReported = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.PathVisitor.prototype.reset"></a>[function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>reset (path)](#apidoc.element.regenerator.types.PathVisitor.prototype.reset)
- description and source-code
```javascript
reset = function (path) {
    // Empty stub; may be reassigned or overridden by subclasses.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.PathVisitor.prototype.visit"></a>[function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>visit ()](#apidoc.element.regenerator.types.PathVisitor.prototype.visit)
- description and source-code
```javascript
visit = function () {
    if (this._visiting) {
        throw new Error(
          "Recursively calling visitor.visit(path) resets visitor state. " +
          "Try this.visit(path) or this.traverse(path) instead."
        );
    }

    // Private state that needs to be reset before every traversal.
    this._visiting = true;
    this._changeReported = false;
    this._abortRequested = false;

    var argc = arguments.length;
    var args = new Array(argc)
    for (var i = 0; i < argc; ++i) {
        args[i] = arguments[i];
    }

    if (!(args[0] instanceof NodePath)) {
        args[0] = new NodePath({root: args[0]}).get("root");
    }

    // Called with the same arguments as .visit.
    this.reset.apply(this, args);

    try {
        var root = this.visitWithoutReset(args[0]);
        var didNotThrow = true;
    } finally {
        this._visiting = false;

        if (!didNotThrow && this._abortRequested) {
            // If this.visitWithoutReset threw an exception and
            // this._abortRequested was set to true, return the root of
            // the AST instead of letting the exception propagate, so that
            // client code does not have to provide a try-catch block to
            // intercept the AbortRequest exception.  Other kinds of
            // exceptions will propagate without being intercepted and
            // rethrown by a catch block, so their stacks will accurately
            // reflect the original throwing context.
            return args[0].value;
        }
    }

    return root;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.PathVisitor.prototype.visitWithoutReset"></a>[function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>visitWithoutReset (path)](#apidoc.element.regenerator.types.PathVisitor.prototype.visitWithoutReset)
- description and source-code
```javascript
visitWithoutReset = function (path) {
    if (this instanceof this.Context) {
        // Since this.Context.prototype === this, there's a chance we
        // might accidentally call context.visitWithoutReset. If that
        // happens, re-invoke the method against context.visitor.
        return this.visitor.visitWithoutReset(path);
    }

    if (!(path instanceof NodePath)) {
        throw new Error("");
    }

    var value = path.value;

    var methodName = value &&
      typeof value === "object" &&
      typeof value.type === "string" &&
      this._methodNameTable[value.type];

    if (methodName) {
        var context = this.acquireContext(path);
        try {
            return context.invokeVisitorMethod(methodName);
        } finally {
            this.releaseContext(context);
        }

    } else {
        // If there was no visitor method to call, visit the children of
        // this node generically.
        return visitChildren(path, this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.PathVisitor.prototype.wasChangeReported"></a>[function <span class="apidocSignatureSpan">regenerator.types.PathVisitor.prototype.</span>wasChangeReported ()](#apidoc.element.regenerator.types.PathVisitor.prototype.wasChangeReported)
- description and source-code
```javascript
wasChangeReported = function () {
    return this._changeReported;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.regenerator.types.Type"></a>[module regenerator.types.Type](#apidoc.module.regenerator.types.Type)

#### <a name="apidoc.element.regenerator.types.Type.Type"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>Type (check, name)](#apidoc.element.regenerator.types.Type.Type)
- description and source-code
```javascript
function Type(check, name) {
    var self = this;
    if (!(self instanceof Type)) {
        throw new Error("Type constructor cannot be invoked without 'new'");
    }

    // Unfortunately we can't elegantly reuse isFunction and isString,
    // here, because this code is executed while defining those types.
    if (objToStr.call(check) !== funObjStr) {
        throw new Error(check + " is not a function");
    }

    // The 'name' parameter can be either a function or a string.
    var nameObjStr = objToStr.call(name);
    if (!(nameObjStr === funObjStr ||
      nameObjStr === strObjStr)) {
        throw new Error(name + " is neither a function nor a string");
    }

    Object.defineProperties(self, {
        name: {value: name},
        check: {
            value: function (value, deep) {
                var result = check.call(self, value, deep);
                if (!result && deep && objToStr.call(deep) === funObjStr)
                    deep(self, value);
                return result;
            }
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Type.def"></a>[function <span class="apidocSignatureSpan">regenerator.types.Type.</span>def (typeName)](#apidoc.element.regenerator.types.Type.def)
- description and source-code
```javascript
def = function (typeName) {
    isString.assert(typeName);
    return hasOwn.call(defCache, typeName)
      ? defCache[typeName]
      : defCache[typeName] = new Def(typeName);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Type.fromArray"></a>[function <span class="apidocSignatureSpan">regenerator.types.Type.</span>fromArray (arr)](#apidoc.element.regenerator.types.Type.fromArray)
- description and source-code
```javascript
fromArray = function (arr) {
    if (!isArray.check(arr)) {
        throw new Error("");
    }
    if (arr.length !== 1) {
        throw new Error("only one element type is permitted for typed arrays");
    }
    return toType(arr[0]).arrayOf();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Type.fromObject"></a>[function <span class="apidocSignatureSpan">regenerator.types.Type.</span>fromObject (obj)](#apidoc.element.regenerator.types.Type.fromObject)
- description and source-code
```javascript
fromObject = function (obj) {
    var fields = Object.keys(obj).map(function (name) {
        return new Field(name, obj[name]);
    });

    return new Type(function (value, deep) {
        return isObject.check(value) && fields.every(function (field) {
              return field.type.check(value[field.name], deep);
          });
    }, function () {
        return "{ " + fields.join(", ") + " }";
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Type.or"></a>[function <span class="apidocSignatureSpan">regenerator.types.Type.</span>or ()](#apidoc.element.regenerator.types.Type.or)
- description and source-code
```javascript
or = function () {
    var types = [];
    var len = arguments.length;
    for (var i = 0; i < len; ++i)
        types.push(toType(arguments[i]));

    return new Type(function (value, deep) {
        for (var i = 0; i < len; ++i)
            if (types[i].check(value, deep))
                return true;
        return false;
    }, function () {
        return types.join(" | ");
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.regenerator.types.Type.prototype"></a>[module regenerator.types.Type.prototype](#apidoc.module.regenerator.types.Type.prototype)

#### <a name="apidoc.element.regenerator.types.Type.prototype.arrayOf"></a>[function <span class="apidocSignatureSpan">regenerator.types.Type.prototype.</span>arrayOf ()](#apidoc.element.regenerator.types.Type.prototype.arrayOf)
- description and source-code
```javascript
arrayOf = function () {
    var elemType = this;
    return new Type(function (value, deep) {
        return isArray.check(value) && value.every(function (elem) {
              return elemType.check(elem, deep);
          });
    }, function () {
        return "[" + elemType + "]";
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.Type.prototype.assert"></a>[function <span class="apidocSignatureSpan">regenerator.types.Type.prototype.</span>assert (value, deep)](#apidoc.element.regenerator.types.Type.prototype.assert)
- description and source-code
```javascript
assert = function (value, deep) {
    if (!this.check(value, deep)) {
        var str = shallowStringify(value);
        throw new Error(str + " does not match type " + this);
    }
    return true;
}
```
- example usage
```shell
...
  injectRuntime(n.File.check(node) ? node.program : node);
}

return node;
};

function injectRuntime(program) {
n.Program.assert(program);

// Include the runtime by modifying the AST rather than by concatenating
// strings. This technique will allow for more accurate source mapping.
var runtimePath = require("..").runtime.path;
var runtime = fs.readFileSync(runtimePath, "utf8");
var runtimeBody = recast.parse(runtime, {
  sourceFileName: runtimePath
...
```

#### <a name="apidoc.element.regenerator.types.Type.prototype.toString"></a>[function <span class="apidocSignatureSpan">regenerator.types.Type.prototype.</span>toString ()](#apidoc.element.regenerator.types.Type.prototype.toString)
- description and source-code
```javascript
toString = function () {
    var name = this.name;

    if (isString.check(name))
        return name;

    if (isFunction.check(name))
        return name.call(this) + "";

    return name + " type";
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.regenerator.types.astNodesAreEquivalent"></a>[module regenerator.types.astNodesAreEquivalent](#apidoc.module.regenerator.types.astNodesAreEquivalent)

#### <a name="apidoc.element.regenerator.types.astNodesAreEquivalent.astNodesAreEquivalent"></a>[function <span class="apidocSignatureSpan">regenerator.types.</span>astNodesAreEquivalent (a, b, problemPath)](#apidoc.element.regenerator.types.astNodesAreEquivalent.astNodesAreEquivalent)
- description and source-code
```javascript
function astNodesAreEquivalent(a, b, problemPath) {
    if (isArray.check(problemPath)) {
        problemPath.length = 0;
    } else {
        problemPath = null;
    }

    return areEquivalent(a, b, problemPath);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.astNodesAreEquivalent.assert"></a>[function <span class="apidocSignatureSpan">regenerator.types.astNodesAreEquivalent.</span>assert (a, b)](#apidoc.element.regenerator.types.astNodesAreEquivalent.assert)
- description and source-code
```javascript
assert = function (a, b) {
    var problemPath = [];
    if (!astNodesAreEquivalent(a, b, problemPath)) {
        if (problemPath.length === 0) {
            if (a !== b) {
                throw new Error("Nodes must be equal");
            }
        } else {
            throw new Error(
              "Nodes differ in the following path: " +
              problemPath.map(subscriptForProperty).join("")
            );
        }
    }
}
```
- example usage
```shell
...
  injectRuntime(n.File.check(node) ? node.program : node);
}

return node;
};

function injectRuntime(program) {
n.Program.assert(program);

// Include the runtime by modifying the AST rather than by concatenating
// strings. This technique will allow for more accurate source mapping.
var runtimePath = require("..").runtime.path;
var runtime = fs.readFileSync(runtimePath, "utf8");
var runtimeBody = recast.parse(runtime, {
  sourceFileName: runtimePath
...
```



# <a name="apidoc.module.regenerator.types.builders"></a>[module regenerator.types.builders](#apidoc.module.regenerator.types.builders)

#### <a name="apidoc.element.regenerator.types.builders.anyTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>anyTypeAnnotation ()](#apidoc.element.regenerator.types.builders.anyTypeAnnotation)
- description and source-code
```javascript
anyTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.arrayExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>arrayExpression ()](#apidoc.element.regenerator.types.builders.arrayExpression)
- description and source-code
```javascript
arrayExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.arrayPattern"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>arrayPattern ()](#apidoc.element.regenerator.types.builders.arrayPattern)
- description and source-code
```javascript
arrayPattern = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.arrayStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>arrayStatement ()](#apidoc.element.regenerator.types.builders.arrayStatement)
- description and source-code
```javascript
arrayStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.arrayTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>arrayTypeAnnotation ()](#apidoc.element.regenerator.types.builders.arrayTypeAnnotation)
- description and source-code
```javascript
arrayTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.arrowFunctionExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>arrowFunctionExpression ()](#apidoc.element.regenerator.types.builders.arrowFunctionExpression)
- description and source-code
```javascript
arrowFunctionExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.arrowFunctionStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>arrowFunctionStatement ()](#apidoc.element.regenerator.types.builders.arrowFunctionStatement)
- description and source-code
```javascript
arrowFunctionStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.assignmentExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>assignmentExpression ()](#apidoc.element.regenerator.types.builders.assignmentExpression)
- description and source-code
```javascript
assignmentExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.assignmentPattern"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>assignmentPattern ()](#apidoc.element.regenerator.types.builders.assignmentPattern)
- description and source-code
```javascript
assignmentPattern = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.assignmentStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>assignmentStatement ()](#apidoc.element.regenerator.types.builders.assignmentStatement)
- description and source-code
```javascript
assignmentStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.awaitExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>awaitExpression ()](#apidoc.element.regenerator.types.builders.awaitExpression)
- description and source-code
```javascript
awaitExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.awaitStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>awaitStatement ()](#apidoc.element.regenerator.types.builders.awaitStatement)
- description and source-code
```javascript
awaitStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.binaryExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>binaryExpression ()](#apidoc.element.regenerator.types.builders.binaryExpression)
- description and source-code
```javascript
binaryExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.binaryStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>binaryStatement ()](#apidoc.element.regenerator.types.builders.binaryStatement)
- description and source-code
```javascript
binaryStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.bindExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>bindExpression ()](#apidoc.element.regenerator.types.builders.bindExpression)
- description and source-code
```javascript
bindExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.bindStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>bindStatement ()](#apidoc.element.regenerator.types.builders.bindStatement)
- description and source-code
```javascript
bindStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.block"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>block ()](#apidoc.element.regenerator.types.builders.block)
- description and source-code
```javascript
block = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.blockStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>blockStatement ()](#apidoc.element.regenerator.types.builders.blockStatement)
- description and source-code
```javascript
blockStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.booleanLiteral"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>booleanLiteral ()](#apidoc.element.regenerator.types.builders.booleanLiteral)
- description and source-code
```javascript
booleanLiteral = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.booleanLiteralStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>booleanLiteralStatement ()](#apidoc.element.regenerator.types.builders.booleanLiteralStatement)
- description and source-code
```javascript
booleanLiteralStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.booleanLiteralTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>booleanLiteralTypeAnnotation ()](#apidoc.element.regenerator.types.builders.booleanLiteralTypeAnnotation)
- description and source-code
```javascript
booleanLiteralTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.booleanTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>booleanTypeAnnotation ()](#apidoc.element.regenerator.types.builders.booleanTypeAnnotation)
- description and source-code
```javascript
booleanTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.breakStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>breakStatement ()](#apidoc.element.regenerator.types.builders.breakStatement)
- description and source-code
```javascript
breakStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.callExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>callExpression ()](#apidoc.element.regenerator.types.builders.callExpression)
- description and source-code
```javascript
callExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.callStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>callStatement ()](#apidoc.element.regenerator.types.builders.callStatement)
- description and source-code
```javascript
callStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.catchClause"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>catchClause ()](#apidoc.element.regenerator.types.builders.catchClause)
- description and source-code
```javascript
catchClause = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.classBody"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classBody ()](#apidoc.element.regenerator.types.builders.classBody)
- description and source-code
```javascript
classBody = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.classDeclaration"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classDeclaration ()](#apidoc.element.regenerator.types.builders.classDeclaration)
- description and source-code
```javascript
classDeclaration = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.classExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classExpression ()](#apidoc.element.regenerator.types.builders.classExpression)
- description and source-code
```javascript
classExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.classImplements"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classImplements ()](#apidoc.element.regenerator.types.builders.classImplements)
- description and source-code
```javascript
classImplements = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.classMethod"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classMethod ()](#apidoc.element.regenerator.types.builders.classMethod)
- description and source-code
```javascript
classMethod = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.classProperty"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classProperty ()](#apidoc.element.regenerator.types.builders.classProperty)
- description and source-code
```javascript
classProperty = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.classPropertyDefinition"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classPropertyDefinition ()](#apidoc.element.regenerator.types.builders.classPropertyDefinition)
- description and source-code
```javascript
classPropertyDefinition = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.classStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>classStatement ()](#apidoc.element.regenerator.types.builders.classStatement)
- description and source-code
```javascript
classStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.commentBlock"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>commentBlock ()](#apidoc.element.regenerator.types.builders.commentBlock)
- description and source-code
```javascript
commentBlock = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.commentLine"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>commentLine ()](#apidoc.element.regenerator.types.builders.commentLine)
- description and source-code
```javascript
commentLine = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.comprehensionBlock"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>comprehensionBlock ()](#apidoc.element.regenerator.types.builders.comprehensionBlock)
- description and source-code
```javascript
comprehensionBlock = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.comprehensionExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>comprehensionExpression ()](#apidoc.element.regenerator.types.builders.comprehensionExpression)
- description and source-code
```javascript
comprehensionExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.comprehensionStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>comprehensionStatement ()](#apidoc.element.regenerator.types.builders.comprehensionStatement)
- description and source-code
```javascript
comprehensionStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.conditionalExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>conditionalExpression ()](#apidoc.element.regenerator.types.builders.conditionalExpression)
- description and source-code
```javascript
conditionalExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.conditionalStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>conditionalStatement ()](#apidoc.element.regenerator.types.builders.conditionalStatement)
- description and source-code
```javascript
conditionalStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.continueStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>continueStatement ()](#apidoc.element.regenerator.types.builders.continueStatement)
- description and source-code
```javascript
continueStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.debuggerStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>debuggerStatement ()](#apidoc.element.regenerator.types.builders.debuggerStatement)
- description and source-code
```javascript
debuggerStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.declareClass"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareClass ()](#apidoc.element.regenerator.types.builders.declareClass)
- description and source-code
```javascript
declareClass = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.declareExportAllDeclaration"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareExportAllDeclaration ()](#apidoc.element.regenerator.types.builders.declareExportAllDeclaration)
- description and source-code
```javascript
declareExportAllDeclaration = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.declareExportDeclaration"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareExportDeclaration ()](#apidoc.element.regenerator.types.builders.declareExportDeclaration)
- description and source-code
```javascript
declareExportDeclaration = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.declareFunction"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareFunction ()](#apidoc.element.regenerator.types.builders.declareFunction)
- description and source-code
```javascript
declareFunction = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.declareInterface"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareInterface ()](#apidoc.element.regenerator.types.builders.declareInterface)
- description and source-code
```javascript
declareInterface = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.declareModule"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareModule ()](#apidoc.element.regenerator.types.builders.declareModule)
- description and source-code
```javascript
declareModule = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.declareModuleExports"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareModuleExports ()](#apidoc.element.regenerator.types.builders.declareModuleExports)
- description and source-code
```javascript
declareModuleExports = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.declareTypeAlias"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareTypeAlias ()](#apidoc.element.regenerator.types.builders.declareTypeAlias)
- description and source-code
```javascript
declareTypeAlias = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.declareVariable"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>declareVariable ()](#apidoc.element.regenerator.types.builders.declareVariable)
- description and source-code
```javascript
declareVariable = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.decorator"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>decorator ()](#apidoc.element.regenerator.types.builders.decorator)
- description and source-code
```javascript
decorator = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.directive"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>directive ()](#apidoc.element.regenerator.types.builders.directive)
- description and source-code
```javascript
directive = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.directiveLiteral"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>directiveLiteral ()](#apidoc.element.regenerator.types.builders.directiveLiteral)
- description and source-code
```javascript
directiveLiteral = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.directiveLiteralStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>directiveLiteralStatement ()](#apidoc.element.regenerator.types.builders.directiveLiteralStatement)
- description and source-code
```javascript
directiveLiteralStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.doExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>doExpression ()](#apidoc.element.regenerator.types.builders.doExpression)
- description and source-code
```javascript
doExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.doStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>doStatement ()](#apidoc.element.regenerator.types.builders.doStatement)
- description and source-code
```javascript
doStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.doWhileStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>doWhileStatement ()](#apidoc.element.regenerator.types.builders.doWhileStatement)
- description and source-code
```javascript
doWhileStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.emptyStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>emptyStatement ()](#apidoc.element.regenerator.types.builders.emptyStatement)
- description and source-code
```javascript
emptyStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.emptyTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>emptyTypeAnnotation ()](#apidoc.element.regenerator.types.builders.emptyTypeAnnotation)
- description and source-code
```javascript
emptyTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.existentialTypeParam"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>existentialTypeParam ()](#apidoc.element.regenerator.types.builders.existentialTypeParam)
- description and source-code
```javascript
existentialTypeParam = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.existsTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>existsTypeAnnotation ()](#apidoc.element.regenerator.types.builders.existsTypeAnnotation)
- description and source-code
```javascript
existsTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.exportAllDeclaration"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportAllDeclaration ()](#apidoc.element.regenerator.types.builders.exportAllDeclaration)
- description and source-code
```javascript
exportAllDeclaration = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.exportBatchSpecifier"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportBatchSpecifier ()](#apidoc.element.regenerator.types.builders.exportBatchSpecifier)
- description and source-code
```javascript
exportBatchSpecifier = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.exportDeclaration"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportDeclaration ()](#apidoc.element.regenerator.types.builders.exportDeclaration)
- description and source-code
```javascript
exportDeclaration = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.exportDefaultDeclaration"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportDefaultDeclaration ()](#apidoc.element.regenerator.types.builders.exportDefaultDeclaration)
- description and source-code
```javascript
exportDefaultDeclaration = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.exportDefaultSpecifier"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportDefaultSpecifier ()](#apidoc.element.regenerator.types.builders.exportDefaultSpecifier)
- description and source-code
```javascript
exportDefaultSpecifier = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.exportNamedDeclaration"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportNamedDeclaration ()](#apidoc.element.regenerator.types.builders.exportNamedDeclaration)
- description and source-code
```javascript
exportNamedDeclaration = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.exportNamespaceSpecifier"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportNamespaceSpecifier ()](#apidoc.element.regenerator.types.builders.exportNamespaceSpecifier)
- description and source-code
```javascript
exportNamespaceSpecifier = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.exportSpecifier"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>exportSpecifier ()](#apidoc.element.regenerator.types.builders.exportSpecifier)
- description and source-code
```javascript
exportSpecifier = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.expressionStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>expressionStatement ()](#apidoc.element.regenerator.types.builders.expressionStatement)
- description and source-code
```javascript
expressionStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.file"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>file ()](#apidoc.element.regenerator.types.builders.file)
- description and source-code
```javascript
file = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.forAwaitStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>forAwaitStatement ()](#apidoc.element.regenerator.types.builders.forAwaitStatement)
- description and source-code
```javascript
forAwaitStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.forInStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>forInStatement ()](#apidoc.element.regenerator.types.builders.forInStatement)
- description and source-code
```javascript
forInStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.forOfStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>forOfStatement ()](#apidoc.element.regenerator.types.builders.forOfStatement)
- description and source-code
```javascript
forOfStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.forStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>forStatement ()](#apidoc.element.regenerator.types.builders.forStatement)
- description and source-code
```javascript
forStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.functionDeclaration"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>functionDeclaration ()](#apidoc.element.regenerator.types.builders.functionDeclaration)
- description and source-code
```javascript
functionDeclaration = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.functionExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>functionExpression ()](#apidoc.element.regenerator.types.builders.functionExpression)
- description and source-code
```javascript
functionExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.functionStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>functionStatement ()](#apidoc.element.regenerator.types.builders.functionStatement)
- description and source-code
```javascript
functionStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.functionTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>functionTypeAnnotation ()](#apidoc.element.regenerator.types.builders.functionTypeAnnotation)
- description and source-code
```javascript
functionTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.functionTypeParam"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>functionTypeParam ()](#apidoc.element.regenerator.types.builders.functionTypeParam)
- description and source-code
```javascript
functionTypeParam = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.generatorExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>generatorExpression ()](#apidoc.element.regenerator.types.builders.generatorExpression)
- description and source-code
```javascript
generatorExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.generatorStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>generatorStatement ()](#apidoc.element.regenerator.types.builders.generatorStatement)
- description and source-code
```javascript
generatorStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.genericTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>genericTypeAnnotation ()](#apidoc.element.regenerator.types.builders.genericTypeAnnotation)
- description and source-code
```javascript
genericTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.graphExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>graphExpression ()](#apidoc.element.regenerator.types.builders.graphExpression)
- description and source-code
```javascript
graphExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.graphIndexExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>graphIndexExpression ()](#apidoc.element.regenerator.types.builders.graphIndexExpression)
- description and source-code
```javascript
graphIndexExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.graphIndexStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>graphIndexStatement ()](#apidoc.element.regenerator.types.builders.graphIndexStatement)
- description and source-code
```javascript
graphIndexStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.graphStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>graphStatement ()](#apidoc.element.regenerator.types.builders.graphStatement)
- description and source-code
```javascript
graphStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.identifier"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>identifier ()](#apidoc.element.regenerator.types.builders.identifier)
- description and source-code
```javascript
identifier = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
...
  }

  return obj;
};

exports.runtimeProperty = function(name) {
  return b.memberExpression(
    b.identifier("regeneratorRuntime"),
    b.identifier(name),
    false
  );
};

// Inspired by the isReference function from ast-util:
// https://github.com/eventualbuddha/ast-util/blob/9bf91c5ce8/lib/index.js#L466-L506
...
```

#### <a name="apidoc.element.regenerator.types.builders.identifierStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>identifierStatement ()](#apidoc.element.regenerator.types.builders.identifierStatement)
- description and source-code
```javascript
identifierStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.ifStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>ifStatement ()](#apidoc.element.regenerator.types.builders.ifStatement)
- description and source-code
```javascript
ifStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.import"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>import ()](#apidoc.element.regenerator.types.builders.import)
- description and source-code
```javascript
import = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.importDeclaration"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>importDeclaration ()](#apidoc.element.regenerator.types.builders.importDeclaration)
- description and source-code
```javascript
importDeclaration = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.importDefaultSpecifier"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>importDefaultSpecifier ()](#apidoc.element.regenerator.types.builders.importDefaultSpecifier)
- description and source-code
```javascript
importDefaultSpecifier = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.importNamespaceSpecifier"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>importNamespaceSpecifier ()](#apidoc.element.regenerator.types.builders.importNamespaceSpecifier)
- description and source-code
```javascript
importNamespaceSpecifier = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.importSpecifier"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>importSpecifier ()](#apidoc.element.regenerator.types.builders.importSpecifier)
- description and source-code
```javascript
importSpecifier = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.importStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>importStatement ()](#apidoc.element.regenerator.types.builders.importStatement)
- description and source-code
```javascript
importStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.interfaceDeclaration"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>interfaceDeclaration ()](#apidoc.element.regenerator.types.builders.interfaceDeclaration)
- description and source-code
```javascript
interfaceDeclaration = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.interfaceExtends"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>interfaceExtends ()](#apidoc.element.regenerator.types.builders.interfaceExtends)
- description and source-code
```javascript
interfaceExtends = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.intersectionTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>intersectionTypeAnnotation ()](#apidoc.element.regenerator.types.builders.intersectionTypeAnnotation)
- description and source-code
```javascript
intersectionTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxAttribute"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxAttribute ()](#apidoc.element.regenerator.types.builders.jsxAttribute)
- description and source-code
```javascript
jsxAttribute = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxClosingElement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxClosingElement ()](#apidoc.element.regenerator.types.builders.jsxClosingElement)
- description and source-code
```javascript
jsxClosingElement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxElement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxElement ()](#apidoc.element.regenerator.types.builders.jsxElement)
- description and source-code
```javascript
jsxElement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxElementStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxElementStatement ()](#apidoc.element.regenerator.types.builders.jsxElementStatement)
- description and source-code
```javascript
jsxElementStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxEmptyExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxEmptyExpression ()](#apidoc.element.regenerator.types.builders.jsxEmptyExpression)
- description and source-code
```javascript
jsxEmptyExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxEmptyStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxEmptyStatement ()](#apidoc.element.regenerator.types.builders.jsxEmptyStatement)
- description and source-code
```javascript
jsxEmptyStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxExpressionContainer"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxExpressionContainer ()](#apidoc.element.regenerator.types.builders.jsxExpressionContainer)
- description and source-code
```javascript
jsxExpressionContainer = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxExpressionContainerStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxExpressionContainerStatement ()](#apidoc.element.regenerator.types.builders.jsxExpressionContainerStatement)
- description and source-code
```javascript
jsxExpressionContainerStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxIdentifier"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxIdentifier ()](#apidoc.element.regenerator.types.builders.jsxIdentifier)
- description and source-code
```javascript
jsxIdentifier = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxIdentifierStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxIdentifierStatement ()](#apidoc.element.regenerator.types.builders.jsxIdentifierStatement)
- description and source-code
```javascript
jsxIdentifierStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxMemberExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxMemberExpression ()](#apidoc.element.regenerator.types.builders.jsxMemberExpression)
- description and source-code
```javascript
jsxMemberExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxMemberStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxMemberStatement ()](#apidoc.element.regenerator.types.builders.jsxMemberStatement)
- description and source-code
```javascript
jsxMemberStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxNamespacedName"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxNamespacedName ()](#apidoc.element.regenerator.types.builders.jsxNamespacedName)
- description and source-code
```javascript
jsxNamespacedName = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxOpeningElement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxOpeningElement ()](#apidoc.element.regenerator.types.builders.jsxOpeningElement)
- description and source-code
```javascript
jsxOpeningElement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxSpreadAttribute"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxSpreadAttribute ()](#apidoc.element.regenerator.types.builders.jsxSpreadAttribute)
- description and source-code
```javascript
jsxSpreadAttribute = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxText"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxText ()](#apidoc.element.regenerator.types.builders.jsxText)
- description and source-code
```javascript
jsxText = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.jsxTextStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>jsxTextStatement ()](#apidoc.element.regenerator.types.builders.jsxTextStatement)
- description and source-code
```javascript
jsxTextStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.labeledStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>labeledStatement ()](#apidoc.element.regenerator.types.builders.labeledStatement)
- description and source-code
```javascript
labeledStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.letExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>letExpression ()](#apidoc.element.regenerator.types.builders.letExpression)
- description and source-code
```javascript
letExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.letStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>letStatement ()](#apidoc.element.regenerator.types.builders.letStatement)
- description and source-code
```javascript
letStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.line"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>line ()](#apidoc.element.regenerator.types.builders.line)
- description and source-code
```javascript
line = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.literal"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>literal ()](#apidoc.element.regenerator.types.builders.literal)
- description and source-code
```javascript
literal = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.literalStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>literalStatement ()](#apidoc.element.regenerator.types.builders.literalStatement)
- description and source-code
```javascript
literalStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.logicalExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>logicalExpression ()](#apidoc.element.regenerator.types.builders.logicalExpression)
- description and source-code
```javascript
logicalExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.logicalStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>logicalStatement ()](#apidoc.element.regenerator.types.builders.logicalStatement)
- description and source-code
```javascript
logicalStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.memberExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>memberExpression ()](#apidoc.element.regenerator.types.builders.memberExpression)
- description and source-code
```javascript
memberExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
...
    }
  }

  return obj;
};

exports.runtimeProperty = function(name) {
  return b.memberExpression(
    b.identifier("regeneratorRuntime"),
    b.identifier(name),
    false
  );
};

// Inspired by the isReference function from ast-util:
...
```

#### <a name="apidoc.element.regenerator.types.builders.memberStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>memberStatement ()](#apidoc.element.regenerator.types.builders.memberStatement)
- description and source-code
```javascript
memberStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.memberTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>memberTypeAnnotation ()](#apidoc.element.regenerator.types.builders.memberTypeAnnotation)
- description and source-code
```javascript
memberTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.metaProperty"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>metaProperty ()](#apidoc.element.regenerator.types.builders.metaProperty)
- description and source-code
```javascript
metaProperty = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.metaPropertyStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>metaPropertyStatement ()](#apidoc.element.regenerator.types.builders.metaPropertyStatement)
- description and source-code
```javascript
metaPropertyStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.methodDefinition"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>methodDefinition ()](#apidoc.element.regenerator.types.builders.methodDefinition)
- description and source-code
```javascript
methodDefinition = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.mixedTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>mixedTypeAnnotation ()](#apidoc.element.regenerator.types.builders.mixedTypeAnnotation)
- description and source-code
```javascript
mixedTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.newExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>newExpression ()](#apidoc.element.regenerator.types.builders.newExpression)
- description and source-code
```javascript
newExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.newStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>newStatement ()](#apidoc.element.regenerator.types.builders.newStatement)
- description and source-code
```javascript
newStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.noop"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>noop ()](#apidoc.element.regenerator.types.builders.noop)
- description and source-code
```javascript
noop = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.nullLiteral"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>nullLiteral ()](#apidoc.element.regenerator.types.builders.nullLiteral)
- description and source-code
```javascript
nullLiteral = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.nullLiteralStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>nullLiteralStatement ()](#apidoc.element.regenerator.types.builders.nullLiteralStatement)
- description and source-code
```javascript
nullLiteralStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.nullLiteralTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>nullLiteralTypeAnnotation ()](#apidoc.element.regenerator.types.builders.nullLiteralTypeAnnotation)
- description and source-code
```javascript
nullLiteralTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.nullTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>nullTypeAnnotation ()](#apidoc.element.regenerator.types.builders.nullTypeAnnotation)
- description and source-code
```javascript
nullTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.nullableTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>nullableTypeAnnotation ()](#apidoc.element.regenerator.types.builders.nullableTypeAnnotation)
- description and source-code
```javascript
nullableTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.numberLiteralTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>numberLiteralTypeAnnotation ()](#apidoc.element.regenerator.types.builders.numberLiteralTypeAnnotation)
- description and source-code
```javascript
numberLiteralTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.numberTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>numberTypeAnnotation ()](#apidoc.element.regenerator.types.builders.numberTypeAnnotation)
- description and source-code
```javascript
numberTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.numericLiteral"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>numericLiteral ()](#apidoc.element.regenerator.types.builders.numericLiteral)
- description and source-code
```javascript
numericLiteral = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.numericLiteralStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>numericLiteralStatement ()](#apidoc.element.regenerator.types.builders.numericLiteralStatement)
- description and source-code
```javascript
numericLiteralStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.numericLiteralTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>numericLiteralTypeAnnotation ()](#apidoc.element.regenerator.types.builders.numericLiteralTypeAnnotation)
- description and source-code
```javascript
numericLiteralTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.objectExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectExpression ()](#apidoc.element.regenerator.types.builders.objectExpression)
- description and source-code
```javascript
objectExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.objectMethod"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectMethod ()](#apidoc.element.regenerator.types.builders.objectMethod)
- description and source-code
```javascript
objectMethod = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.objectPattern"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectPattern ()](#apidoc.element.regenerator.types.builders.objectPattern)
- description and source-code
```javascript
objectPattern = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.objectProperty"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectProperty ()](#apidoc.element.regenerator.types.builders.objectProperty)
- description and source-code
```javascript
objectProperty = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.objectStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectStatement ()](#apidoc.element.regenerator.types.builders.objectStatement)
- description and source-code
```javascript
objectStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.objectTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectTypeAnnotation ()](#apidoc.element.regenerator.types.builders.objectTypeAnnotation)
- description and source-code
```javascript
objectTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.objectTypeCallProperty"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectTypeCallProperty ()](#apidoc.element.regenerator.types.builders.objectTypeCallProperty)
- description and source-code
```javascript
objectTypeCallProperty = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.objectTypeIndexer"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectTypeIndexer ()](#apidoc.element.regenerator.types.builders.objectTypeIndexer)
- description and source-code
```javascript
objectTypeIndexer = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.objectTypeProperty"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>objectTypeProperty ()](#apidoc.element.regenerator.types.builders.objectTypeProperty)
- description and source-code
```javascript
objectTypeProperty = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.parenthesizedExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>parenthesizedExpression ()](#apidoc.element.regenerator.types.builders.parenthesizedExpression)
- description and source-code
```javascript
parenthesizedExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.parenthesizedStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>parenthesizedStatement ()](#apidoc.element.regenerator.types.builders.parenthesizedStatement)
- description and source-code
```javascript
parenthesizedStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.position"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>position ()](#apidoc.element.regenerator.types.builders.position)
- description and source-code
```javascript
position = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.program"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>program ()](#apidoc.element.regenerator.types.builders.program)
- description and source-code
```javascript
program = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.property"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>property ()](#apidoc.element.regenerator.types.builders.property)
- description and source-code
```javascript
property = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.propertyPattern"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>propertyPattern ()](#apidoc.element.regenerator.types.builders.propertyPattern)
- description and source-code
```javascript
propertyPattern = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.qualifiedTypeIdentifier"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>qualifiedTypeIdentifier ()](#apidoc.element.regenerator.types.builders.qualifiedTypeIdentifier)
- description and source-code
```javascript
qualifiedTypeIdentifier = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.regExpLiteral"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>regExpLiteral ()](#apidoc.element.regenerator.types.builders.regExpLiteral)
- description and source-code
```javascript
regExpLiteral = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.regExpLiteralStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>regExpLiteralStatement ()](#apidoc.element.regenerator.types.builders.regExpLiteralStatement)
- description and source-code
```javascript
regExpLiteralStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.restElement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>restElement ()](#apidoc.element.regenerator.types.builders.restElement)
- description and source-code
```javascript
restElement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.restProperty"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>restProperty ()](#apidoc.element.regenerator.types.builders.restProperty)
- description and source-code
```javascript
restProperty = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.returnStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>returnStatement ()](#apidoc.element.regenerator.types.builders.returnStatement)
- description and source-code
```javascript
returnStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.sequenceExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>sequenceExpression ()](#apidoc.element.regenerator.types.builders.sequenceExpression)
- description and source-code
```javascript
sequenceExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.sequenceStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>sequenceStatement ()](#apidoc.element.regenerator.types.builders.sequenceStatement)
- description and source-code
```javascript
sequenceStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.sourceLocation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>sourceLocation ()](#apidoc.element.regenerator.types.builders.sourceLocation)
- description and source-code
```javascript
sourceLocation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.spreadElement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>spreadElement ()](#apidoc.element.regenerator.types.builders.spreadElement)
- description and source-code
```javascript
spreadElement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.spreadElementPattern"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>spreadElementPattern ()](#apidoc.element.regenerator.types.builders.spreadElementPattern)
- description and source-code
```javascript
spreadElementPattern = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.spreadProperty"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>spreadProperty ()](#apidoc.element.regenerator.types.builders.spreadProperty)
- description and source-code
```javascript
spreadProperty = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.spreadPropertyPattern"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>spreadPropertyPattern ()](#apidoc.element.regenerator.types.builders.spreadPropertyPattern)
- description and source-code
```javascript
spreadPropertyPattern = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.stringLiteral"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>stringLiteral ()](#apidoc.element.regenerator.types.builders.stringLiteral)
- description and source-code
```javascript
stringLiteral = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.stringLiteralStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>stringLiteralStatement ()](#apidoc.element.regenerator.types.builders.stringLiteralStatement)
- description and source-code
```javascript
stringLiteralStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.stringLiteralTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>stringLiteralTypeAnnotation ()](#apidoc.element.regenerator.types.builders.stringLiteralTypeAnnotation)
- description and source-code
```javascript
stringLiteralTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.stringTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>stringTypeAnnotation ()](#apidoc.element.regenerator.types.builders.stringTypeAnnotation)
- description and source-code
```javascript
stringTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.super"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>super ()](#apidoc.element.regenerator.types.builders.super)
- description and source-code
```javascript
super = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.superStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>superStatement ()](#apidoc.element.regenerator.types.builders.superStatement)
- description and source-code
```javascript
superStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.switchCase"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>switchCase ()](#apidoc.element.regenerator.types.builders.switchCase)
- description and source-code
```javascript
switchCase = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.switchStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>switchStatement ()](#apidoc.element.regenerator.types.builders.switchStatement)
- description and source-code
```javascript
switchStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.taggedTemplateExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>taggedTemplateExpression ()](#apidoc.element.regenerator.types.builders.taggedTemplateExpression)
- description and source-code
```javascript
taggedTemplateExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.taggedTemplateStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>taggedTemplateStatement ()](#apidoc.element.regenerator.types.builders.taggedTemplateStatement)
- description and source-code
```javascript
taggedTemplateStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.templateElement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>templateElement ()](#apidoc.element.regenerator.types.builders.templateElement)
- description and source-code
```javascript
templateElement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.templateLiteral"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>templateLiteral ()](#apidoc.element.regenerator.types.builders.templateLiteral)
- description and source-code
```javascript
templateLiteral = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.templateLiteralStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>templateLiteralStatement ()](#apidoc.element.regenerator.types.builders.templateLiteralStatement)
- description and source-code
```javascript
templateLiteralStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.thisExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>thisExpression ()](#apidoc.element.regenerator.types.builders.thisExpression)
- description and source-code
```javascript
thisExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.thisStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>thisStatement ()](#apidoc.element.regenerator.types.builders.thisStatement)
- description and source-code
```javascript
thisStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.thisTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>thisTypeAnnotation ()](#apidoc.element.regenerator.types.builders.thisTypeAnnotation)
- description and source-code
```javascript
thisTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.throwStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>throwStatement ()](#apidoc.element.regenerator.types.builders.throwStatement)
- description and source-code
```javascript
throwStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.tryStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>tryStatement ()](#apidoc.element.regenerator.types.builders.tryStatement)
- description and source-code
```javascript
tryStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.tupleTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>tupleTypeAnnotation ()](#apidoc.element.regenerator.types.builders.tupleTypeAnnotation)
- description and source-code
```javascript
tupleTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.typeAlias"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeAlias ()](#apidoc.element.regenerator.types.builders.typeAlias)
- description and source-code
```javascript
typeAlias = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.typeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeAnnotation ()](#apidoc.element.regenerator.types.builders.typeAnnotation)
- description and source-code
```javascript
typeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.typeCastExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeCastExpression ()](#apidoc.element.regenerator.types.builders.typeCastExpression)
- description and source-code
```javascript
typeCastExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.typeCastStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeCastStatement ()](#apidoc.element.regenerator.types.builders.typeCastStatement)
- description and source-code
```javascript
typeCastStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.typeParameter"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeParameter ()](#apidoc.element.regenerator.types.builders.typeParameter)
- description and source-code
```javascript
typeParameter = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.typeParameterDeclaration"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeParameterDeclaration ()](#apidoc.element.regenerator.types.builders.typeParameterDeclaration)
- description and source-code
```javascript
typeParameterDeclaration = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.typeParameterInstantiation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeParameterInstantiation ()](#apidoc.element.regenerator.types.builders.typeParameterInstantiation)
- description and source-code
```javascript
typeParameterInstantiation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.typeofTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>typeofTypeAnnotation ()](#apidoc.element.regenerator.types.builders.typeofTypeAnnotation)
- description and source-code
```javascript
typeofTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.unaryExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>unaryExpression ()](#apidoc.element.regenerator.types.builders.unaryExpression)
- description and source-code
```javascript
unaryExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.unaryStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>unaryStatement ()](#apidoc.element.regenerator.types.builders.unaryStatement)
- description and source-code
```javascript
unaryStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.unionTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>unionTypeAnnotation ()](#apidoc.element.regenerator.types.builders.unionTypeAnnotation)
- description and source-code
```javascript
unionTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.updateExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>updateExpression ()](#apidoc.element.regenerator.types.builders.updateExpression)
- description and source-code
```javascript
updateExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.updateStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>updateStatement ()](#apidoc.element.regenerator.types.builders.updateStatement)
- description and source-code
```javascript
updateStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.variableDeclaration"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>variableDeclaration ()](#apidoc.element.regenerator.types.builders.variableDeclaration)
- description and source-code
```javascript
variableDeclaration = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.variableDeclarator"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>variableDeclarator ()](#apidoc.element.regenerator.types.builders.variableDeclarator)
- description and source-code
```javascript
variableDeclarator = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.voidTypeAnnotation"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>voidTypeAnnotation ()](#apidoc.element.regenerator.types.builders.voidTypeAnnotation)
- description and source-code
```javascript
voidTypeAnnotation = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.whileStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>whileStatement ()](#apidoc.element.regenerator.types.builders.whileStatement)
- description and source-code
```javascript
whileStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.withStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>withStatement ()](#apidoc.element.regenerator.types.builders.withStatement)
- description and source-code
```javascript
withStatement = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.yieldExpression"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>yieldExpression ()](#apidoc.element.regenerator.types.builders.yieldExpression)
- description and source-code
```javascript
yieldExpression = function () {
    var args = arguments;
    var argc = args.length;
    var built = Object.create(nodePrototype);

    if (!self.finalized) {
        throw new Error(
          "attempting to instantiate unfinalized type " +
          self.typeName
        );
    }

    function add(param, i) {
        if (hasOwn.call(built, param))
            return;

        var all = self.allFields;
        if (!hasOwn.call(all, param)) {
            throw new Error("" + param);
        }

        var field = all[param];
        var type = field.type;
        var value;

        if (isNumber.check(i) && i < argc) {
            value = args[i];
        } else if (field.defaultFn) {
            // Expose the partially-built object to the default
            // function as its 'this' object.
            value = field.defaultFn.call(built);
        } else {
            var message = "no value or default function given for field " +
              JSON.stringify(param) + " of " + self.typeName + "(" +
              self.buildParams.map(function (name) {
                  return all[name];
              }).join(", ") + ")";
            throw new Error(message);
        }

        if (!type.check(value)) {
            throw new Error(
              shallowStringify(value) +
              " does not match field " + field +
              " of type " + self.typeName
            );
        }

        // TODO Could attach getters and setters here to enforce
        // dynamic type safety.
        built[param] = value;
    }

    self.buildParams.forEach(function (param, i) {
        add(param, i);
    });

    Object.keys(self.allFields).forEach(function (param) {
        add(param); // Use the default value.
    });

    // Make sure that the "type" field was filled automatically.
    if (built.type !== self.typeName) {
        throw new Error("");
    }

    return built;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.types.builders.yieldStatement"></a>[function <span class="apidocSignatureSpan">regenerator.types.builders.</span>yieldStatement ()](#apidoc.element.regenerator.types.builders.yieldStatement)
- description and source-code
```javascript
yieldStatement = function () {
    return builders.expressionStatement(wrapped.apply(builders, arguments));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.regenerator.util"></a>[module regenerator.util](#apidoc.module.regenerator.util)

#### <a name="apidoc.element.regenerator.util.defaults"></a>[function <span class="apidocSignatureSpan">regenerator.util.</span>defaults (obj)](#apidoc.element.regenerator.util.defaults)
- description and source-code
```javascript
defaults = function (obj) {
  var len = arguments.length;
  var extension;

  for (var i = 1; i < len; ++i) {
    if ((extension = arguments[i])) {
      for (var key in extension) {
        if (hasOwn.call(extension, key) && !hasOwn.call(obj, key)) {
          obj[key] = extension[key];
        }
      }
    }
  }

  return obj;
}
```
- example usage
```shell
...
  plugins: ["*", "jsx", "flow"]
}
};

function compile(source, options) {
var result;

options = utils.defaults(options || {}, {
  includeRuntime: false
});

// Shortcut: Transform only if generators or async functions present.
if (genOrAsyncFunExp.test(source)) {
  result = require("babel-core").transform(source, transformOptions);
} else {
...
```

#### <a name="apidoc.element.regenerator.util.isReference"></a>[function <span class="apidocSignatureSpan">regenerator.util.</span>isReference (path, name)](#apidoc.element.regenerator.util.isReference)
- description and source-code
```javascript
isReference = function (path, name) {
  var node = path.value;

  if (!n.Identifier.check(node)) {
    return false;
  }

  if (name && node.name !== name) {
    return false;
  }

  var parent = path.parent.value;

  switch (parent.type) {
  case "VariableDeclarator":
    return path.name === "init";

  case "MemberExpression":
    return path.name === "object" || (
      parent.computed && path.name === "property"
    );

  case "FunctionExpression":
  case "FunctionDeclaration":
  case "ArrowFunctionExpression":
    if (path.name === "id") {
      return false;
    }

    if (path.parentPath.name === "params" &&
        parent.params === path.parentPath.value &&
        parent.params[path.name] === node) {
      return false;
    }

    return true;

  case "ClassDeclaration":
  case "ClassExpression":
    return path.name !== "id";

  case "CatchClause":
    return path.name !== "param";

  case "Property":
  case "MethodDefinition":
    return path.name !== "key";

  case "ImportSpecifier":
  case "ImportDefaultSpecifier":
  case "ImportNamespaceSpecifier":
  case "LabeledStatement":
    return false;

  default:
    return true;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.regenerator.util.runtimeProperty"></a>[function <span class="apidocSignatureSpan">regenerator.util.</span>runtimeProperty (name)](#apidoc.element.regenerator.util.runtimeProperty)
- description and source-code
```javascript
runtimeProperty = function (name) {
  return b.memberExpression(
    b.identifier("regeneratorRuntime"),
    b.identifier(name),
    false
  );
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.regenerator.visit"></a>[module regenerator.visit](#apidoc.module.regenerator.visit)

#### <a name="apidoc.element.regenerator.visit.transform"></a>[function <span class="apidocSignatureSpan">regenerator.visit.</span>transform (node, options)](#apidoc.element.regenerator.visit.transform)
- description and source-code
```javascript
function transform(node, options) {
  options = util.defaults(options || {}, {
    includeRuntime: false
  });

  var result = require("babel-core").transformFromAst(node, null, {
    presets: [require("regenerator-preset")],
    code: false,
    ast: true
  });

  node = result.ast;

  if (options.includeRuntime === true) {
    injectRuntime(n.File.check(node) ? node.program : node);
  }

  return node;
}
```
- example usage
```shell
...
}).code;
'''

AST transformation:
'''js
var recast = require("recast");
var ast = recast.parse(es6Source);
ast = require("regenerator").transform(ast);
var es5Source = recast.print(ast);
'''

How can you get involved?
---

The easiest way to get involved is to look for buggy examples using [the
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
