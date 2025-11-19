# 虚拟环境
## 创建
```bash
#项目根目录下创建 .venv
python -m venv .venv
```
-m 把后面的参数当作一个模块（module）来运行，而不是脚本文件。  
### 为什么用 -m venv 而不是直接 venv？
因为：
- 你的系统可能没有把 venv 加到 PATH（它不是一个独立可执行文件）
- 但只要你装了 Python ≥3.3，venv 模块就一定在标准库里
- 用 python -m venv 能确保使用当前 python 命令对应的 Python 版本来创建环境

## 激活
```bash
# Windows 激活
.venv\Scripts\activate

# macOS/Linux 激活
source .venv/bin/activate
```

## 退出
```bash
deactivate
```