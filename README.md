# Custom Git Commands

## Description

- These are some custom git commands
- They automate some of the tedious commands developers use daily
- They essentially package a few commands together for more efficient 'git'ing

## Setup

### Mac
- Put the parent directory in your PATH:
  ```
  export PATH="$HOME/Code/custom-git-commands:$PATH"
  ```
- Restart your terminal:
  ```
  source ~/.zshrc
  ```

### Windows
- Put the parent directory in your PATH:
  ```
  setx PATH "%PATH%;%USERPROFILE%\Code\custom-git-commands"
  ```
- Restart your terminal by closing and reopening it

## How to use

To run one of the commands, simply type out the file name with the arguments if necessary:

### Mac
```
git-lazy-push "This is a commit message"
```

### Windows
```
git lazy-push "This is a commit message"
```

## Git aliases

- Short aliases for everyday commands, in `aliases.gitconfig`
- Include them once, pointing at wherever you cloned this:
  ```
  git config --global include.path "$PWD/aliases.gitconfig"
  ```
- Git merges them with any aliases you already have

## Create your own

- To create your own command follow the following steps:

1. touch git-<your command name>
2. chmod +x <above file>
3. vim <file>
4. Edit file using the other commands as a reference
5. Restart your terminal
6. Enjoy

### Happy 'git'ing!
