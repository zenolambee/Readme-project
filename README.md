# Readme-project

## OpenCode configuration

Copy this JSON into `/root/.config/opencode/opencode.json`:

```json
{
  "$schema": "https://opencode.ai/config.json",
  "provider": {
    "nvidia": {
      "npm": "@ai-sdk/openai-compatible",
      "name": "NVIDIA Gateway",
      "options": {
        "baseURL": "http://43.153.225.102:3000/v1"
      },
      "models": {
        "coding": {
          "name": "step-3.7-flash"
        },
        "cohere/north-mini-code:free": {
          "name": "North Mini Code Free"
        },
        "deepseek-ai/deepseek-v4-flash": {
          "name": "DeepSeek V4 Flash"
        },
        "deepseek-ai/deepseek-v4-pro": {
          "name": "DeepSeek V4 Pro"
        },
        "openai/gpt-oss-20b:free": {
          "name": "GPT-OSS 20B Free"
        },
        "google/gemma-4-26b-a4b-it:free": {
          "name": "Gemma 4 26B Free"
        },
        "z-ai/glm-5.2": {
          "name": "GLM 5.2"
        },
        "minimax/minimax-m2.7": {
          "name": "MiniMax M2.7"
        },
        "mistralai/mistral-medium-3.5-12b": {
          "name": "Mistral Medium 3.5"
        },
        "stepfun/step-3.7-flash": {
          "name": "Step 3.7 Flash"
        },
        "bytedance-seed/seed-2.0-lite": {
          "name": "Seed 2.0 Lite"
        }
      }
    },
    "buatprem": {
      "npm": "@ai-sdk/openai-compatible",
      "name": "BuatPrem",
      "options": {
        "baseURL": "https://autoapp.biz.id/v1"
      },
      "models": {
        "glm-5.2": {
          "name": "glm-5.2"
        },
        "kimi-k2.7-code": {
          "name": "kimi-k2.7-code"
        },
        "deepseek-v4-pro": {
          "name": "deepseek-v4-pro"
        },
        "kimi-k2.7-code-highspeed": {
          "name": "kimi-k2.7-code-highspeed"
        },
        "auto": {
          "name": "auto"
        },
        "gpt-5.5": {
          "name": "gpt-5.5"
        },
        "gpt-5.6": {
          "name": "gpt-5.6"
        },
        "mistral-large-3-675b-instruct": {
          "name": "mistral-large-3-675b-instruct"
        },
        "deepseek-v4-flash": {
          "name": "deepseek-v4-flash"
        },
        "gpt-5.6-sol": {
          "name": "gpt-5.6-sol"
        },
        "gpt-5.6-terra": {
          "name": "gpt-5.6-terra"
        },
        "gpt-5.6-luna": {
          "name": "gpt-5.6-luna"
        },
        "kimi-k3": {
          "name": "kimi-k3"
        },
        "deepseek-v4-mod": {
          "name": "deepseek-v4-mod"
        },
        "claude-sonnet-5": {
          "name": "claude-sonnet-5"
        },
        "claude-opus-4.8": {
          "name": "claude-opus-4.8"
        },
        "gpt-5.6-sol-xhigh": {
          "name": "gpt-5.6-sol-xhigh"
        },
        "claude-opus-5": {
          "name": "claude-opus-5"
        },
        "auto-debug": {
          "name": "auto-debug"
        }
      }
    }
  },
  "model": "apiproxy/step-3.7-flash"
}
```

## Notes

- Use the JSON above as the main OpenCode config.
- Save it exactly in `/root/.config/opencode/opencode.json`.
- Adjust `baseURL` only if your gateway address changes.
