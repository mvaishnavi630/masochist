---
tags: git
cache_breaker: 1
---

[Git 1.5.5.1](/wiki/Git_1.5.5.1) was released on or about 21 April 2008.

## Release notes

This is a local copy of the [official release notes](http://repo.or.cz/w/git.git?a=blob;f=Documentation/RelNotes-1.5.5.1.txt;h=7de419708f77fff6f61e749b917b5fcecbe9a292;hb=5909ca92d8b2c6a0534597f52f7733ff61a64d63):

    GIT v1.5.5.1 Release Notes
    ==========================

    Fixes since v1.5.5
    ------------------

     * "git archive --prefix=$path/" mishandled gitattributes.

     * "git fetch -v" that fetches into FETCH_HEAD did not report the summary
       the same way as done for updating the tracking refs.

     * "git svn" misbehaved when the configuration file customized the "git
       log" output format using format.pretty.

     * "git submodule status" leaked an unnecessary error message.

     * "git log --date-order --topo-order" did not override the earlier
       date-order with topo-order as expected.

     * "git bisect good $this" did not check the validity of the revision
       given properly.

     * "url.<there>.insteadOf" did not work correctly.

     * "git clean" ran inside subdirectory behaved as if the directory was
       explicitly specified for removal by the end user from the top level.

     * "git bisect" from a detached head leaked an unnecessary error message.

     * "git bisect good $a $b" when $a is Ok but $b is bogus should have
       atomically failed before marking $a as good.

     * "git fmt-merge-msg" did not clean up leading empty lines from commit
       log messages like "git log" family does.

     * "git am" recorded a commit with empty Subject: line without
       complaining.

     * when given a commit log message whose first paragraph consists of
       multiple lines, "git rebase" squashed it into a single line.

     * "git remote add $bogus_name $url" did not complain properly.

    Also comes with various documentation updates.

## See also

-   [Upgrading to Git 1.5.5.1](/wiki/Upgrading_to_Git_1.5.5.1)
