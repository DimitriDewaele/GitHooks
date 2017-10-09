# GitHooks

This repository is used to experiment with hooks.

# Informational

 - All Git hooks are ordinary scripts that Git executes when certain events occur.
 - Hooks can reside in either local or server-side repositories.
 - Hooks are not under version control. This means that they work local on the client or server, where they reside.
 - You can put the hooks in a folder under version control, and use them with a reference.
 - Local hooks: developers can change them.
 - Server hooks: Activated on the server: push, pull, ...
 

# Version History

 - v0.1 **git commit**: Initial commit on local machine: initializes the .git/hooks/*.sample --> A git init will create default sample hooks.
 - v0.2 **git commit**: Acitvate hook: prepare-commit-msg and look at the commit message. --> remove the .sample and the hook will become active.
 - v0.3 Add hooks in the repo. This is an alternative way to add hooks and put them in the repo.
	 - Add the hooks in directory /hooks/
	 - Use the hooks by setting: git config core.hooksPath hooks