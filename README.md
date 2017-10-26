Template
========

[![Latest version][Version image]][Releases]
[![Total downloads][Downloads image]][Downloads]
[![Build status][Build image]][Build]
[![Test coverage][Coverage image]][Coverage]
[![Code style][Style image]][Style]

Template for creating new ScriptFUSION projects.

Usage
-----

1. `git clone git@github.com:ScriptFUSION/Template.git MYPROJ` &ndash; Clone this repository as *MYPROJ*.
2. `(shopt -s dotglob; for file in *.dist; do mv "$file" "${file%.*}"; done)` &ndash; Rename `*.dist` files, removing the *.dist* extension.
3.
    1. Create a hosted repository for the project on a VCS service like GitHub and note its URL.
    2. `git remote set-url origin MYURL` &ndash; Change the origin URL to *MYURL*.
4. Replace placeholders in `composer.json`.
5. Generate a new readme with `bin/generate readme template` or edit manually.
6. `git add . && git commit -m 'Initial commit.'` &ndash; Commit changes.
7. `git push` &ndash; Upload changes.


  [Releases]: https://github.com/ScriptFUSION/Template/releases
  [Version image]: https://poser.pugx.org/scriptfusion/template/version "Latest version"
  [Downloads]: https://packagist.org/packages/scriptfusion/template
  [Downloads image]: https://poser.pugx.org/scriptfusion/template/downloads "Total downloads"
  [Build]: https://travis-ci.org/ScriptFUSION/Template
  [Build image]: https://travis-ci.org/ScriptFUSION/Template.svg?branch=master "Build status"
  [Coverage]: https://coveralls.io/github/ScriptFUSION/Template
  [Coverage image]: https://coveralls.io/repos/ScriptFUSION/Template/badge.svg "Test coverage"
  [Style]: https://styleci.io/repos/94649077
  [Style image]: https://styleci.io/repos/94649077/shield?style=flat "Code style"
