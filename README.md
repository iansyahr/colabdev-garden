# colabdev-garden
A collection of code cheatsheets for setting up different tools, libraries, programming languages, etc. on Google Colab

## Index
- [Deno](#deno)
- [Esbuild](#esbuild)
- [Go](#go)
- [Node.js & npm](#nodejs--npm)
- [Rust](#rust)

### Deno
```python
import os
os.system("curl -fsSL https://deno.land/install.sh | sh")
os.environ['PATH'] += ":/root/.deno/bin/"
```

### Esbuild

```python
import os
os.system("curl -fsSL https://esbuild.github.io/dl/latest | sh")
os.environ['PATH'] += ":/content/"
```

### Go

```python
import os
os.system("wget https://go.dev/dl/go1.21.0.linux-amd64.tar.gz")
os.system("rm -rf /root/go/bin && tar -C /root -xzf go1.21.0.linux-amd64.tar.gz")
os.environ['PATH'] += ":/root/go/bin"
```
### Node.js & npm

```python
import os
os.system("wget https://nodejs.org/dist/v18.17.1/node-v18.17.1-linux-x64.tar.xz")
os.system("tar -xf node-v18.17.1-linux-x64.tar.xz")
os.system("mv node-v18.17.1-linux-x64 node")
os.system("rm -rf /tools/node && mv node /tools")
os.environ['PATH'] += ":/tools/node/bin"
```

### Rust

```python
import os
os.system("curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y")
os.environ['PATH'] += ":/root/.cargo/bin"
```
