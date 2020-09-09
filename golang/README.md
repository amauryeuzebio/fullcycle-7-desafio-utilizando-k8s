### Pré requisitos
- Instalação docker.

### Build da imagem
```docker
docker build . -t desafio-k8s
```

### Executar a imagem
```docker
docker run -p 8000:8000 --rm desafio-k8s