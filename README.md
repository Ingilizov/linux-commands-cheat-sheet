# Linux Commands Cheat Sheet: With Examples

* Create a new file and its parent directories if necessary
  ```bash
  # with mkdir
  mkdir -p /path/to && echo "some data" > $_/file.txt
  
  # without mkdir
  echo "some data" | install -D /dev/stdin /path/to/file.txt
  ```

* rm: device or resource busy - Find the PID of the Process and kill it. Than delete file or dir.

  ```bash
  ps -Af | grep 'file-or-process-name' | awk '{ print $2 }' | xargs kill
  ```
