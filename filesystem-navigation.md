# Filesystem Navigation

Linux is organized around a hierarchical filesystem. Before working with files, applications, logs, or system configuration, it is important to understand how to identify your current location and navigate between directories.

---

## `pwd` — Print Working Directory

Displays the full path of the directory you are currently working in.

```bash
pwd
```

Example output:

```text
/home/chris
```

This is useful for confirming your location in the filesystem before navigating to another directory or working with files.

---

## `ls` — List Directory Contents

Displays the files and directories contained within the current directory.

```bash
ls
```

Example:

```text
Documents  Downloads  Projects
```

`ls` can also be used to view the contents of another directory without navigating into it:

```bash
ls /var
```

---

## `cd` — Change Directory

Changes the current working directory.

```bash
cd Documents
```

The current location can then be verified with:

```bash
pwd
```

Example output:

```text
/home/chris/Documents
```

---

## `cd ..` — Move Up One Directory

`..` represents the parent directory of the current location.

For example, when working in:

```text
/home/chris/Documents
```

Running:

```bash
cd ..
```

moves back to:

```text
/home/chris
```

---

## Practical Example

A simple navigation workflow might look like:

```bash
pwd
ls
cd Documents
pwd
ls
cd ..
pwd
```

This provides a basic workflow for identifying the current location, inspecting available directories, navigating into a directory, and returning to its parent.
