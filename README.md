# AMD Agent Zero

Agente de IA autónomo optimizado para GPU AMD ROCm.

## Uso

```bash
docker run -d \
  --name agent-zero \
  --device /dev/kfd \
  --device /dev/dri \
  -e HSA_OVERRIDE_GFX_VERSION=10.3.0 \
  -e LLM_MODEL=qwen2.5:14b \
  -p 8000:8000 \
  ghcr.io/drmicalet/arch-amd-agent-zero:latest
```

## Requisitos

- GPU AMD RDNA2/RDNA3
- ROCm 6.x
- 12GB+ VRAM

## Descarga

```bash
docker pull ghcr.io/drmicalet/arch-amd-agent-zero:latest
```

## Licencia

GPL-3.0

## Autor

**Drmicalet** - [GitHub](https://github.com/Drmicalet)
