# qwode
**Collaboration notice:** Ali Azam, Promita Rahee Sikder

Qwen 3-4B turned into a code-generating language model by solving a bunch of programming problems and optimizing a binary correctness signals (from its test execution) using GRPO-style reinforcement learning.

## Usage
Run the sandbox:
```bash
docker run -it -p 8080:8080 -v ./sandbox_config/local.yaml:/root/sandbox/sandbox/configs/local.yaml volcengine/sandbox-fusion:server-20250609
```

Install dependencies using uv (the superior `pip`):
```bash
uv sync
```
or
```bash
pip install -r requirements.txt
```

And then run:
```bash
uv run train.py max_steps=250
```
or

```bash
python train.py max_steps=250
```
