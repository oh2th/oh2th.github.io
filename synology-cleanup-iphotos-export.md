# Cleanup shell commands after an export from Apple Photos to Synology

Moves almbum folders one step up from the city/date folders.

```
for i in 2019*; do (cd $i && find . -maxdepth 2 -type f -not -path "./\@eaDir/*" -exec mv {} . \;); done
```

Next cleanup the Synology @eaDir metadata and caches.

```
find . -type d -name "\@eaDir" -exec rm -rf {} \;
```

Finally delete all remmaining empty folders.

```
find . -type d -empty -exec rm -r {} \;
```

You may need to execute the last two commands as long as no errors are found.
