Usage:

  ```
  black_and_white [action] [...]

  black_and_white
  black_and_white play
  black_and_white install
  black_and_white configure
  black_and_white backup
  black_and_white restore
  black_and_white backup [name]
  black_and_white restore [name]
  ```

Without arguments, `play` is the implied action.  `play` implies `install` as a
prior action.  `install` acts only if the game is not yet installed.
`configure` provides controls for screen resolution.  `backup` backs up
profiles and creatures.  A name for the backup may be specified.  `restore`
restores a backup (destructively).  A backup may be specified by name.  If no
name is specified, the most recent backup file is restored.
