# Developing conventions for Git
## Commits
* Commit message:
    * Consists of: `Verb: message`
    * _message_ consists of:
        * _subjects_ -  method, function, class, object or variable or construction, and so on. 
        * _utility words_ - describe what commit do
* **One _subject_ - one commit message!**
* When, in some reasons there is more than one _subject_ affected in commit, you can list them one by one with comma. 
    
* Prepend commit messages with determinative _verbs_:
    * `Add:`      - when _add_ a new _subject_ 
    * `Remove:`   - when _remove_ some _subject_
    * `Move`      - when _subject_ was moved
    * `Rename`    - when _subject_ was renamed
    * `Improve`   - when _add_ some functionality from _subject_
    * `Refactor:` - when _refactor_ some _subject_
    * `Fix:`      - when _fix_ some errors or behavior for _subject_
    * `Typo:`     - when _fix_ some typo in code
    
    * `Spec:_verb_:` - all _verbs_ described higher for specs
    
* Example _subjects_ for which _verbs_ are applied:
    * `Module::`
    * `ClassName`
    * `ClassName#instance_method_name`
    * `ClassName.class_method_name`
    * `ClassName@instance_varible`
    * `'unless'`, `'if'`
    * `commentary` - comments for _subject_
    * `file.md`
    
* Example _utility words_:
    * `=>_subject_name_` - shows what _subject_ returns
    * `make _subject_` - make _subject_ to do something 
    * `param '_param_name_'` - param with _param_name 
    * `for _subject_`  - add something for _subject_
    * `from _subject_` - remove something for _subject_
    * `in _subject_` - some internal changes in _subject_
    * `_subject_ to _subject_new_` - replace _subject_ with another _subject_ or change name of the _subject_
    * `case` - some case for _subject_ (expectially for _Spec:_ _verb_)
    * `missed` - some missed _subject_
    
* Common patterns:
    * `Fix: make ChangelogFetcher#filename =>nil`
    * `Add: 'gem_name' param for ChangelogFetcher`
    * `Move: git.md, ruby.md to /dev/git.txt, /dev/ruby.txt`
