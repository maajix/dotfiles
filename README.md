# Installation using stow

- Move the dotfiles into a folder within the home directory
- Run the following command to create all the symlinks using stow

```bash
$ stow .
```

# Structure of stow

- The dotfiles folder has to have the same structure as from the home folder

```bash
home/kali/.config/.somefile
dotfiles/.config/.somefile
```

- Easy command for moving files after they are copied to the dotfiles directory (replaces conflicting files in the original directory)

```bash
$ stow --adopt .
```

# Adding new files to the ignore list 

```bash
$ echo ".myfile" > .stow-local-ignore
```
