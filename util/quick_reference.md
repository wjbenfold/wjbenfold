# Commands / snippets

## Cherrypicking

```
git checkout <branch>
git remote add <other-fork-alias> <other-fork-URL>
git fetch <other-fork-alias>
git cherry-pick <commit-hash>
git push <your-fork-alias>
```

## Linux

```
# Size of files
du -h --max-depth=1 /my/dir
watch df -h

# SSH
ssh-keygen
ssh-copy-id <user@newmachine>
hostname -A   # What's this machine?
```

## Profiling

```
# cProfile
cProfile.run("main()", "cprofile.out")

# pstats
import sys
import pstats
p = pstats.Stats(sys.argv[1])
p.sort_stats('cumulative').print_stats(20)
p.print_callers(.5, "reshape")

# snakeviz
snakeviz cprofile.out

# See also memray, py-spy
```
