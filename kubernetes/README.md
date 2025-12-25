# opencode-kubernetes

Kubernetes troubleshooting workspace using the Kubernetes MCP server for OpenCode in read-only mode to detect, analyze, and provide remediation suggestions for cluster issues. See [AGENTS.md](AGENTS.md) for detailed guidelines.

## Ollama Setup for Gemma3:12b

1. **Install and run the model**:
   ```bash
   ollama serve
   ollama run gemma3:12b
   ```

2. **Configure k8sgpt**:
   ```bash
   k8sgpt auth add --backend ollama --model gemma3:12b --baseurl http://localhost:11434/v1
   ```
