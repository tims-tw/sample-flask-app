# Exercise 2 - Secret Scanning

## Secret detection with Git hooks

For this exercise, running the application is not necessary.

### 02-01 Talisman

1. Follow the [Talisman installation instructions](00_setup.md#Installing_Talisman)

2. In our sample application, create the file `web/config.py` in a text editor of your choice and add something like `password = 'hello'` to the file and save it.

3. Do a git add of the file. e.g. `git add web/config.py`.

Then do a git commit. e.g. `git commit -m "testing talisman"`

If all is working, you should be prompted by talisman about a potential secret being checked-in.

You can then unstage your changes and checkout all files to revert your local repository to it's previous state.

For example:

```sh
git reset
git checkout .
```
