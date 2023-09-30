# CodeMirror: Odin

- https://odin-lang.org
- https://codemirror.net/examples/lang-package/
- https://lezer.codemirror.net

### Tree Sitter

- https://github.com/lezer-parser/import-tree-sitter

### Related Odin Implementations

- Tree Sitter
	- https://github.com/ap29600/tree-sitter-odin
	- https://github.com/MineBill/tree-sitter-odin
- Vim
	- https://github.com/Tetralux/odin.vim

### Similar Languages

- CodeMirror/Lezer
	- https://github.com/jared-hughes/codemirror-lang-zig
- Tree Sitter
	- https://github.com/maxxnino/tree-sitter-zig
- Vim

## CodeMirror 6 language package template

This is an example repository containing a minimal [CodeMirror](https://codemirror.net/6/) language support package. The idea is to clone it, rename it, and edit it to create support for a new language.

Things you'll need to do (see the [language support example](https://codemirror.net/6/examples/lang-package/) for a more detailed tutorial):

 * `git grep EXAMPLE` and replace all instances with your language name.

 * Rewrite the grammar in `src/syntax.grammar` to cover your language. See the [Lezer system guide](https://lezer.codemirror.net/docs/guide/#writing-a-grammar) for information on this file format.

 * Adjust the metadata in `src/index.ts` to work with your new grammar.

 * Adjust the grammar tests in `test/cases.txt`.

 * Build (`npm run prepare`) and test (`npm test`).

 * Rewrite this readme file.

 * Optionally add a license.

 * Publish. Put your package on npm under a name like `codemirror-lang-EXAMPLE`.
