# What's the command to display the 10 most used commands?

```sh
history | awk '{for (i=4; i<=NF; i++) printf "%s ", $i; print ""}' | sort | uniq -c | sort -nr | head -n 10
```
