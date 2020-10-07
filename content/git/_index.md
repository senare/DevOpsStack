
+++
title = "GIT"
outputs = ["Reveal"]
+++

# GIT

---

[![GIT](/senare/images/git.png)](https://git-scm.com/docs)

[[github-git-cheat-sheet]](https://training.github.com/downloads/github-git-cheat-sheet/)

[[git-cheatsheet]](https://ndpsoftware.com/git-cheatsheet.html)

---

{{< slide background-image="/senare/images/git/branches.png" >}}

 - Fast (mostly local operations)
 - Small (each branch is NOT a full copy)
 - Creating branches is cheap
 - Merge branches is cheap
 - Dispose branches is cheap

---

{{< slide background-image="/senare/images/git/branches.png" >}}

- By convention, we single out one branch and call it master (main)

---

{{< slide background-image="/senare/images/git/benevolent-dictator.png" >}}

- Linux kernel development workflow

---

{{< slide background-image="/senare/images/git/integration-manager.png" >}}

- FOSS development workflow

---

{{< slide background-image="/senare/images/git/origin.png" >}}

- Shared repository development workflow 
- All instances are equal
- By convention, we single out one remote and call it origin

---

{{% section %}}

- The data model that Git uses ensures the cryptographic integrity of every bit of your project. 
- Every file and commit is checksummed and retrieved by its checksum when checked back out.
- It is also impossible to change date, commit message, history or any other data in a Git repository without changing the IDs of everything after it.

---

This means that if you have a commit ID, you can be assured not only that your project is exactly the same as when it was committed, but that nothing in its history was changed.

---

This also means you can't push (publish) unless you first pull (download)

---

Unless, ofc you use '-force' (overwrite)

{{% /section %}}

---

{{% section %}}

Merge strategy

---

 Merge

---

 Rebase

---

{{% /section %}}

---

{{% section %}}

Review ( & test ) is more work than writing the code

---

Pull Request

---

Tell your story ... 

---

{{% /section %}}

---
{{% section %}}

 ## Branch strategy

---

[[Git flow]](https://nvie.com/posts/a-successful-git-branching-model/)

---

{{< slide background-image="/senare/images/git/git-flow.png" >}}

---

[[Github flow]](https://guides.github.com/introduction/flow/)

[[Gitlab flow]](https://docs.gitlab.com/ee/topics/gitlab_flow.html)

---

{{< slide background-image="/senare/images/git/simple-git-flow.png" >}}

---

## Library

- Incremental version
- Internal only

---

## Web Application / Server

Web apps are typically continuously delivered, not rolled back, and you don't have to support multiple versions of the software running in the wild.

---

## Application / Client

If, you are building software that is explicitly versioned, or if you need to support multiple versions of your software in the wild.

---

{{% /section %}}

---

# End

[return]({{% relref "/#" %}})


