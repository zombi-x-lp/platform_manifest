## Getting Started ##
---------------
To initialize your local repository using the ZOMBI ROM trees, use a command like this:

    repo init -u git://github.com/zombi-x/platform_manifest.git -b mm6.0
    
Then to sync up:

    repo sync

## Maintaining Authorship ##
----------------------
Mainting authorship is a very important aspect of working with Open Source code. If you wish to submit a patch/fix
from anywhere else (another ROM, project, etc.), it is imperative that you maintain the ownership of the person whose
work you're seeking to include. Doing so will ensure that credit is given where it is deserved, and the [prinicples of open source](http://opensource.org/docs/osd)
are upheld. Your contribution to the project will still be recognized as you will forever be listed as the committer.

If you manually cherry pick a patch/fix then you will need to add the original author prior to pushing to our [gerrit](https://gerrit.omnirom.org).
This is a very easy task to perform, and is usually done after you commit a patch/fix locally. This is accomplished
after you type in `git commit -a` , type in the commit message and save. You would then do the following:

```bash
git commit --amend --author "Author <email@address.com>"
```

So it should look like this once you get all of the author's information

```bash
git commit --amend --author "Spencer McGillicuddy <spencer.the.bestest@gmail.com>"
```

Alternatively, adding as part of the original `git commit` message is preferred and done like the following:

```bash
git commit --author="Author <email@address.com>" -m "[commit message]"
```

This saves time, and when part of your normal routine, prevents the infamous "ermahgerd I forgot to add authorship -
let me fix it because I was found out!" message.
