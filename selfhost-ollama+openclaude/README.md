**Uso básico (porta aleatória, modelo padrão):**
```python
!curl -fsSL "https://raw.githubusercontent.com/JempUnkn/colab-tools/main/selfhost-ollama%2Bopenclaude/run" | bash
```

**Porta específica:**
```python
!curl -fsSL "https://raw.githubusercontent.com/JempUnkn/colab-tools/main/selfhost-ollama%2Bopenclaude/run" | bash -s -- --port 43945
```

**Modelo diferente:**
```python
!curl -fsSL "https://raw.githubusercontent.com/JempUnkn/colab-tools/main/selfhost-ollama%2Bopenclaude/run" | bash -s -- --model llama3.1:8b
```

**Tudo junto:**
```python
!curl -fsSL "https://raw.githubusercontent.com/JempUnkn/colab-tools/main/selfhost-ollama%2Bopenclaude/run" | bash -s -- --port 43945 --model qwen2.5-coder:7b
```

O output final vai ser prox. assim:
```
╔══════════════════════════════════════════════════════════╗
║                    ✅  READY                             ║
╠══════════════════════════════════════════════════════════╣
║  Model     : qwen2.5-coder:7b
║  Base URL  : http://bore.pub:43915/v1
╚══════════════════════════════════════════════════════════╝

  export CLAUDE_CODE_USE_OPENAI=1
  export OPENAI_BASE_URL=http://bore.pub:43915/v1
  export OPENAI_MODEL=qwen2.5-coder:7b

  openclaude
```
