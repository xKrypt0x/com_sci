# Initialise new github repo from CLI

[Bowman, 2020 - Create and Initialize New Github Repo from Command Line](https://dev.to/bowmanjd/create-and-initialize-a-new-github-repository-from-the-command-line-85e)

This method has the advantage of performing all steps from the command line. Meaning no switching back and forth between browser and ide.

### **1**

```
git init
```
### **2**

```
mkdir <directory_name> / touch <file_name>
```

### **3**

```
git add .
```

### **4**

```
git commit -m "<add_message_here>
```
[Git commit message guide](https://www.conventionalcommits.org/en/v1.0.0/)

### **5**

```
curl -u USER_NAME https://api.github.com/user/repo -d '{"name":"NEW_REPO_NAME","private":true/false}'
```

### **6**

```
git add remote origin https://github.com/USER/NEW_REPO_NAME.git
```
### **7**

```
git branch -m master main
```
This moves (-m) the branch history from master to main

### **8**

```
git push -u origin main
```
This pushes main branch to remote, createing an upstream (-u) connection.