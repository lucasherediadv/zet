To apply new environment settings (e.g, updated `$PATH` from `~/.bashrc`) without restarting the terminal:

```sh
exec bash -l
```

* The `-l` flag is crucial, as it forces the shell to be a **login shell**, which re-runs configurations files like `~/.bashrc`.
* The `exec` command replaces the current shell with a new one, inheriting the process ID, which is much faster and more efficient that restarting the terminal application.
* The process is **additive**, this means new environment variables or paths added to your configuration will be present.
