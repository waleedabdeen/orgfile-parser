# orgfile-parser
A parser for org files used in org mode (EMACS)

## Requirements

1. Parse files used by org mode with the extension *.org
2. Write the results as JSON.
3. The JSON file should have the following structure
```   
TASKS  
 |--| description, deadline, schedule, tags, .... |
 |
 |

```

## Related projects

### org-parser project

Can be found here https://github.com/200ok-ch/org-parser

I run it using the following instructions

1. clone the project 

2. You'll need to install the following packages in emacs:
  - clojure-mode - a major mode for editing Clojure and ClojureScript code
  - CIDER - a Clojure interactive development environment and REPL for Emacs
  - projectile(optional) - for navigating inside your projects swiftly

3. Install leiningen from https://leiningen.org/

4. run 

#+begin_src sh :results verbatim :exports both
  lein run test/org_parser/fixtures/schedule_with_repeater.org
#+end_src


## Langauage

Clojure

## Contributors
Waleed Abdeen