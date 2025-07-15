# 🎬 Guia de Otimização de Vídeos para Hero

## Especificações Recomendadas

### Tamanho e Resolução
- **Resolução**: 1920x1080 (Full HD)
- **Proporção**: 16:9
- **Duração**: 10-30 segundos (loop)
- **Tamanho**: máximo 10MB

### Configurações Técnicas
- **Codec**: H.264 (MP4)
- **Framerate**: 30fps
- **Bitrate**: 2-5 Mbps
- **Áudio**: Remover (não é necessário)

## Ferramentas de Otimização

### Online (Gratuito)
1. **CloudConvert**: https://cloudconvert.com/
2. **FreeConvert**: https://www.freeconvert.com/video-compressor
3. **VideoSmaller**: https://www.videosmaller.com/

### Desktop
1. **HandBrake** (Gratuito): https://handbrake.fr/
2. **FFmpeg** (Linha de comando):
   ```bash
   # Comprimir vídeo
   ffmpeg -i input.mp4 -vcodec libx264 -crf 28 -preset medium -vf scale=1920:1080 -an output.mp4
   
   # Converter para WebM
   ffmpeg -i input.mp4 -vcodec libvpx-vp9 -b:v 2M -vf scale=1920:1080 -an output.webm
   ```

## Dicas de Performance

### 1. Preload
```html
<video preload="metadata" ...>
```

### 2. Poster (Imagem de Fallback)
```html
<video poster="./assets/images/hero-poster.jpg" ...>
```

### 3. Lazy Loading
```html
<video loading="lazy" ...>
```

### 4. Múltiplos Formatos
```html
<video>
  <source src="video.webm" type="video/webm">
  <source src="video.mp4" type="video/mp4">
</video>
```

## Exemplo Final Otimizado

```html
<video 
  autoplay 
  loop 
  muted 
  playsinline 
  preload="metadata"
  poster="./assets/images/hero-poster.jpg"
  class="absolute z-0 w-auto min-w-full min-h-full max-w-none"
>
  <source src="./assets/videos/hero-video.webm" type="video/webm">
  <source src="./assets/videos/hero-video.mp4" type="video/mp4">
  Seu navegador não suporta a tag de vídeo.
</video>
```

## Checklist Final

- [ ] Vídeo otimizado (< 10MB)
- [ ] Resolução 1920x1080
- [ ] Duração 10-30 segundos
- [ ] Formato MP4 + WebM
- [ ] Sem áudio
- [ ] Poster image criada
- [ ] Testado em diferentes navegadores
- [ ] Testado em mobile 