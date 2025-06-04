### 1. Creating a New Repository

#### On GitHub
1. Go to [GitHub](https://github.com/) and log in.
2. Click the **New Repository** button.
3. Enter a repository name and description, then click **Create repository**.

#### Locally
```sh
git init my-repo
cd my-repo
```

---

### 2. Cloning a Repository

#### Using HTTPS
```sh
git clone https://github.com/username/repository.git
```

#### Using SSH
```sh
git clone git@github.com:username/repository.git
```

---

### 3. Pushing Changes

```sh
git add .
git commit -m "Your commit message"
git push origin main
```

---

### 4. Pulling Changes

```sh
git pull origin main
```

---

### 5. Setting up SSH

1. Generate an SSH key:
    ```sh
    ssh-keygen -t ed25519 -C "your_email@example.com"
    ```
2. Add the SSH key to your GitHub account:
    - Copy the public key using `cat ~/.ssh/id_ed25519.pub`
    - Go to GitHub > Settings > SSH and GPG keys > New SSH key

---

### 6. Switching Between HTTPS and SSH

- **To set remote to SSH:**
    ```sh
    git remote set-url origin git@github.com:username/repository.git
    ```
- **To set remote to HTTPS:**
    ```sh
    git remote set-url origin https://github.com/username/repository.git
    ```
