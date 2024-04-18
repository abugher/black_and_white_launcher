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
  black_and_white backup_creature <profile name> [creature name]
  black_and_white restore_creature <profile name> [creature name]
  ```

Without arguments, `play` is the implied action.  `play` implies `install` as a
prior action.  `install` acts only if the game is not yet installed.
`configure` provides controls for screen resolution.  `backup` backs up
profiles and creatures.  A name for the backup may be specified.  `restore`
restores a backup (destructively).  A backup may be specified by name.  If no
name is specified, the most recent backup file is restored.  `backup_creature`
backs up the creature from the specified profile.  The creature will be saved
with the specified creature name, if any, or else the in-game name of the
creature.  `restore_creature` restores a creature to the specified profile.  If
no creature name is specified, and only one creature is backed up for this
profile, that creature will be restored.  If multiple creatures are backed up,
a creature name must be specified, and the named creature will be restored.  It
will become the active creature associated with the named profile.
