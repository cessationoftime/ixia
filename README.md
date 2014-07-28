n6
=====

Haskell IDE, with Nix as the primary build method, and Reactive-Banana-WX GUI.  Will look into using cloud-haskell for async ops. Would like  D-language support in the IDE after Haskell.

---

Pull requests: This project will require a contributor license agreement (CLA) to be signed before I will merge pull requests.  But you are not required to sign this to fork/modify the code on your own.


To build with cabal alone:

```bash
git clone https://github.com/cessationoftime/n6.git
cd n6
cabal sandbox init
cabal configure
cabal build
cabal run
```

To build with Nix:

```bash
git clone https://github.com/cessationoftime/n6.git
cd n6
# Activate your Nix profile
source ~/.nix-profile/etc/profile.d/nix.sh
# Update Nix expressions
nix-channel --update
#update packages of user profile from downloaded Nix expressions
nix-env -u '*'
# and build
nix-build
```

Nix Info
* Good [tutorial](http://lethalman.blogspot.it/2014/07/nix-pill-4-basics-of-language.html) on the basics of Nix expressions 
* To setup Nix on Ubuntu/Debian read [this](http://lethalman.blogspot.com/2014/07/nix-pill-2-install-on-your-running.html) or [this](https://www.domenkozar.com/2014/01/02/getting-started-with-nix-package-manager/).


