# Breath — A lost art, rediscovered

Um PWA minimalista com as 12 técnicas de respiração do apêndice de *Breath* de James Nestor.

## Arquivos do repositório

```
breath/
├── index.html                  # app inteiro (HTML + CSS + JS)
├── manifest.webmanifest        # manifest PWA
├── service-worker.js           # cache offline
├── icon-192.png                # ícone
├── icon-512.png                # ícone grande
└── icon-512-maskable.png       # ícone adaptativo Android
```

Zero build, zero dependência. Só soltar na Vercel, GitHub Pages, Netlify ou qualquer host estático.

## Instalar como app

### Android (Chrome/Edge)
Abra o site → menu (três pontos) → **"Instalar app"** ou **"Adicionar à tela inicial"**. O Chrome só mostra a opção quando o service worker já cacheou os recursos, então pode ser que apareça depois de alguns segundos na primeira visita.

### iPhone/iPad (Safari)
Abra no Safari (tem que ser Safari — Chrome no iOS não permite instalar PWAs) → botão de compartilhar → **"Adicionar à Tela de Início"**.

### Desktop (Chrome/Edge)
Barra de endereço mostra um ícone de instalação à direita. Clique nele.

## Deploy na Vercel

1. Suba os arquivos no GitHub
2. Na Vercel, importe o repo
3. Framework preset: **Other** (ou deixe auto)
4. Build command: deixe vazio
5. Output directory: deixe vazio (raiz)

**Importante**: PWAs só funcionam em HTTPS. Vercel e GitHub Pages fornecem HTTPS automaticamente.

## Funcionalidades

- 12 técnicas de respiração com timers precisos
- Sino de transição (Web Audio, gerado em tempo real)
- Drone zen opcional (três osciladores em quinta justa)
- Voz-guia opcional em pt-BR ou en-GB
- Control Pause interativo que alimenta automaticamente o Mini Breathhold
- Persistência local das preferências
- Funciona offline após primeira visita

## Créditos

Baseado no apêndice *Breathing Methods* de **Breath: The New Science of a Lost Art** — James Nestor (2020).
