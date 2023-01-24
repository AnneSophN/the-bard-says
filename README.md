# The bard says

A repository to test **rebasing** and **conflict resolution** in Git

### Exercise

Start the exercise by forking and cloning the repository.

The `story` branch represents a feature branch that is to be rebased.

On the `haiku` branch you find a script that prints a haiku:

```shell
$ python3 main.py

A very short story:


      For sale:
        baby shoes,
        never used...

      by Ernest Hemingway.
```

The short story is great but the
commit history on
the `story` branch is not (on purpose):

```shell
$ git log --all --decorate --oneline --graph


* 8e25704 (HEAD -> story, origin/story) Commit main.py and story.py
| * 6020278 (origin/main, origin/HEAD) Create main.py
|/  
* 0b86855 (main) Add README
* 1d2bfe8 Initial commit

```

Your task is to rebase the `story` branch on top
of `master`.

Verify the history and also that the script still works after the operation.
