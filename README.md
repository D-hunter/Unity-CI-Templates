<!--
Search keywords: Unity CI/CD, Unity GitHub Actions, Unity automation pipeline, Unity build system, Unity deploy GitHub, Unity test automation, Unity game dev CI.
-->

# 🚀 Unity CI/CD Pipeline

**Robust GitHub Actions workflows for Unity projects. Automates testing, multi-platform builds, and GitHub Releases with modular, reusable design.**

![CI](https://github.com/D-hunter/CI-CD-Unity-Test-Project/actions/workflows/ci-cd-pipeline.yml/badge.svg)
![License](https://img.shields.io/github/license/D-hunter/CI-CD-Unity-Test-Project?color=blue)
![Unity](https://img.shields.io/badge/unity-2022.3%2B-black?logo=unity)
![Latest Release](https://img.shields.io/github/v/release/D-hunter/Unity-CI-Templates)

## 🌐 WebGL Demo

See a live WebGL build deployed using this CI/CD pipeline:

➡️ [**Play the Demo**](https://avalin.github.io/Unity-CI-Templates/)

> Deployed via GitHub Pages using the `gh-pages` deploy target.


## 🚀 Getting Started

1️⃣ Ensure your Unity project is in a GitHub repository  
2️⃣ Copy the required GitHub Actions workflows from the [CICD_Workflows folder](https://github.com/D-hunter/Unity-CI-Templates/tree/main/CICD_Workflows)  
3️⃣ Add them to your repository at path: **.github → workflows** _(create folders if missing)_<br/>
4️⃣ Configure the [required secrets](https://github.com/D-hunter/Unity-CI-Templates/wiki/Required-Secrets) in your repository<br/>
5️⃣ Read and optionally setup [repository variables](https://github.com/D-hunter/Unity-CI-Templates/wiki/Repository-Variables), they're important to understand the inputs for the workflow dispatch<br/>
6️⃣ Try dispatching the `ci-cd-dispatcher.yml` workflow or push a Git tag using [SemVer](https://github.com/D-hunter/Unity-CI-Templates/wiki/Versioning-&-Tagging) to see the pipeline in action! <br/>

> ⚠️ Currently tested deploy targets: `gh-pages` (WebGL only). Others are implemented but not yet fully verified. Contributions welcome!

### 🚀 Advanced CI Setup
🐳💻 <strong>Optional: Self-Hosted GitHub Runner with Docker</strong>

Want to run Unity builds on your own hardware? Set up a **Docker-powered GitHub Actions runner**:

**📋 Quick Setup Guide:**
- 🔗 **Repository:** [myoung34/docker-github-actions-runner](https://github.com/myoung34/docker-github-actions-runner)
- 🐳 **Method:** Docker containerization for easy deployment
- ⚙️ **Benefits:** Custom build environments & hardware control

**💡 Perfect for:**
- 💻 Running Unity builds on your own powerful hardware
- 🛠️ Custom build environments with specific tools/dependencies  
- 🔒 Private/secure build environments behind firewalls

</details>

## 📖 Documentation

For full setup instructions, deployment target guides, and advanced configuration tips, see the ➡️ [Wiki](https://github.com/D-hunter/Unity-CI-Templates/wiki)

## 📌 Features

| Feature                        | Description |
|-------------------------------|-------------|
| 🧪 **Test Detection**            | Auto-detects and runs EditMode & PlayMode tests. |
| 🛠️ **Cross-Platform Builds**     | Android, iOS, WebGL, macOS, Windows, and Linux supported. |
| 📦 **Release Deployment**        | Automatically creates GitHub Releases on tag push. |
| 🧹 **Modular Design**            | Fully split into reusable `workflow_call` templates. |
| ⚡ **Parallel Matrix Builds**     | Parallel jobs across macOS and Ubuntu runners. |
| 🔐 **Secure License Activation** | Unity `.ulf` license securely injected during CI. |
| 🗃️ **LFS & Cache**               | Optional Git LFS + caching of Unity `Library` and `Packages/`. |
| 🎛️ **Manual Dispatch**          | Manually trigger preview builds with JSON platform control. |
| 🚀 **Deploy**                | Upload builds to external platforms like itch.io, TestFlight, or custom servers |
| 📣 **Notifications**         | Discord/Slack webhook support |
| 🔍 **Static Analysis**       | C# linters or Unity analyzers |

</details>

## ⚠ Current Limitations

While the pipeline is production-ready and modular, some deploy integrations are still marked as **experimental**:

- 🚧 **Deploy targets like Steam, TestFlight, App Center**  
  These are implemented but have not yet been fully validated in live release pipelines.

- 🔗 **External platforms may require manual setup**  
  Some targets (like itch.io, Firebase, S3) require correctly configured secrets and accounts - be sure to test deploy flows in a safe sandbox environment before pushing to production.

- 🧪 **Unity version compatibility**  
  Currently optimized for Unity 2022.3+, tested with Unity 6 too, but older versions may work as well.

> **Contributions and testing feedback are welcome!**  
> If you successfully validate additional targets or add new ones, please consider opening a PR to improve support for the community.

---

## 🙌 Credits

Crafted with ❤️ by [Avalin](https://github.com/Avalin)  
Powered by GitHub Actions + Unity + Tears.
(PRs welcome!)

