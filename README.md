# Codespace Base (My own implementation)

This repository is a **ready-to-use GitHub Codespace** setup fors HTML, CSS, JavaScript, and Java. Everything you need is pre-installed. No local setup required, though you're free to do so.

---

## **Quick Start**

1. **Fork this repository**  
   - Click the **Fork** button on GitHub.

2. **Create a Codespace**  
   - Open your forked repo on GitHub.
   - Go to **https://github.com/codespaces/new?repo=<YOUR_USERNAME>/codespace-base**. (Remove the <>)
   - Your setting should be as such: ![Settings](/src/settings_image.png)
   - Wait a few minutes while the container builds. It will install:
     - Node.js & npm
     - Java 17
     - Git
     - `http-server`
     - VS Code extensions for HTML, CSS, JS, and Java

3. **Open the terminal**  
   - Check your tools (test commands in bash):
```bash
node -v
npm -v
java -version
http-server --version
git --version
```

4. **Test a simple project**  
```bash
mkdir web-test
echo "<h1>Hello Codespace</h1>" > web-test/index.html
cd web-test
http-server
```
   - Click the forwarded port link in Codespaces to see your page in the browser.

---

## **Tips**

- Find all your Codespaces: [https://github.com/codespaces](https://github.com/codespaces)  
- Save your work often using Git:
```bash
git add .
git commit -m "My first changes"
git push
```
- If you did the last one, then: Don't be worried about your terminal breaking.

---

## **How to do this on your own :)**

- [GitHub Codespaces Documentation](https://docs.github.com/en/codespaces)  
- [Dev Containers Documentation](https://containers.dev/)  
- [VS Code Remote Development](https://code.visualstudio.com/docs/remote/containers)  
- [Dockerfile Reference](https://docs.docker.com/engine/reference/builder/)
