<h1 align="center">Theos server</h1>
<h3 align="center">Set up a macOS sever with <a href="https://github.com/theos/theos">Theos</a> installed using GiHub Actions.</h3>

----

# Before starting
Please read the [GiHub Action Terms of Service](https://docs.github.com/en/github/site-policy/github-additional-product-terms#5-actions-and-packages).

In short, if you're using this project, the software project you're working on must be in the same repository where this GitHub Action is used.

# Usage
1. Visit [this link](https://github.com/raspberryenvoie/theos-server/generate) to generate your repository from this one.\
Or on your existing repository, create a new workflow with [this content](https://raw.githubusercontent.com/raspberryenvoie/theos-server/master/.github/workflows/main.yml).
2. On your repository, go to the Actions tab, choose in the dropdown menu the workflow named `Theos server` and select `Run workflow`.
3. After around 10 secondes you will see an orange cercle. Click on the link next to it.
4. After that, wait a minute and the tmate session will be opened and you will see something like this.
```
WebURL: https://tmate.io/t/urRkvvNuJqBqSwrDMLp49E7zD
SSH: ssh urRkvvNuJqBqSwrDMLp49E7zD@sfo2.tmate.io
```
5. Copy and paste `ssh something.tmate.io` into your terminal (on Windows, use Putty and write `something.tmate.io` in the Host Name field) to connect to the server via SSH.

Notes:
- All the files and directories contained in your repository will be available on the server.
- Don't do anything sensitive on the server such as typing password because anyone could access the server. Store them in [encrypted secrets](https://docs.github.com/en/actions/configuring-and-managing-workflows/creating-and-storing-encrypted-secrets).
- If your repository isn't public, you will have a limit of 2,000 mins of GitHub Actions usage in private repositories.

# Credits
- [Theos](https://github.com/theos) for [Theos](https://github.com/theos/theos)
- [mxschmitt](https://github.com/mxschmitt) for [action-tmate](https://github.com/mxschmitt/action-tmate)
- [xybp888](https://github.com/xybp888) for the patched [iOS-SDKs](https://github.com/xybp888/iOS-SDKs)
