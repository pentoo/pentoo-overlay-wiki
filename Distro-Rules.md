<a href="http://pentoo.ch"><img src="https://github.com/pentoo/pentoo-overlay/wiki/images/pentoo1.png"></a>
### Introduction
We need a set of rules to govern our behavior. This wiki page is intended to be a place to compile such policies in one place.

### USE flags:
pentoo is used to switch on and off our changes to packages we are overriding for gentoo. For instance we have acpid in our repo, and the diffs from gentoo are controlled with the pentoo use flag. livecd is used for things which belong on the livecd but not on the installed systems !livecd is used for things which belong on the running systems but not on the livecd (do not abuse this for large packages) missing we need a new use flag to denote the difference between livecd sized versions and maxi versions. maxi is possible and not currently in use, thoughts? mpentoo will be reserved for a theoretical tiny pentoo like we used to have while minimal will be avoided because of the overlap on gentoo (also minimal doesn't really make sense as a difference between large and huge imho, as well as the fact that building the livecd with minimal would have undesirable consequences like vim being built without gentoo-syntax etc etc). Still taking thoughts...

### Keywording:
Any packages we are overriding from gentoo MUST keep the same keywords as gentoo at all times (do the best you can). Remember when overriding gentoo packages you MUST use the pentoo use flag for all changes. You can always update portage/profiles/package.accept_keywords to install the version you want.

Any packages that are ONLY in pentoo can be keyworded as you please. If you have tested it on an arch then feel free to add that keyword. If you think it is stable, then feel free to keyword it as such.

### Additions:
Please feel free to add to this list of rules and policies as you see fit. Discussion can take place on irc or the dev mailing list.