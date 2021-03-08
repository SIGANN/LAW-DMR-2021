# LAW-DMR-2021
The Joint 15th Linguistic Annotation and 3rd Designing Meaning Representations Workshop

This is the `master` branch; it contains sources for building the website.
The [website](https://sigann.github.io/LAW-XV-2021) itself lives on the `gh-pages` branch.
To deploy changes:

    $ git checkout master
    # ...make, commit, and push changes...
    $ python3 build.py deploy
    $ git checkout gh-pages
    $ mv deploy/* .
    $ rmdir deploy
    $ git commit -a -m "deploy changes"
    $ git push


NB: Only edit the files under `pages/`, since these are the ones used by the build script. Any HTML files in the repository root will be overwritten on deployment.
