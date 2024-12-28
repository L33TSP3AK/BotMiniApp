---
layout: home

hero:
  name: L33TSP3AK Elite
  text: A Private - Blackhat Compilation Utility
  tagline: Advanced Tools for Elite Operators
  image:
    src: https://cdn3.emoji.gg/emojis/7102_NukeExplosion.gif
    alt: Explosion
  actions:
    - theme: brand
      text: Enter the Void
      link: https://t.me/L33TSP3AK_Elite_Bot
    - theme: alt
      text: Access Repository
      link: https://github.com/darknet-elite/core
features:
  - icon: 💳
    title: Financial Services
    details: Advanced card validation, bank verification, and IVR balance checking systems
  - icon: ⚙️
    title: Configuration Tools
    details: Comprehensive suite of configuration management and automation tools
  - icon: 🔍
    title: Search Tools
    details: Advanced search capabilities across multiple data sources and formats
  - icon: 📧
    title: Request Services
    details: Automated request handling and processing with advanced targeting
---

<style>
:root {
  --vp-home-hero-name-color: transparent;
  --vp-home-hero-name-background: -webkit-linear-gradient(120deg, #ff0000 30%, #00e5ff);
  --vp-home-hero-image-background-image: linear-gradient( -45deg, #00ff00 50%, #00e5ff 50% );
  --vp-home-hero-image-filter: blur(72px);
}

@keyframes glitch-skew {
  0% { transform: skew(0deg); }
  20% { transform: skew(-2deg); }
  40% { transform: skew(2deg); }
  60% { transform: skew(-1deg); }
  80% { transform: skew(3deg); }
  100% { transform: skew(0deg); }
}

@keyframes glitch {
  0% {
    clip-path: polygon(0 2%, 100% 2%, 100% 5%, 0 5%);
    transform: translate(0) skew(0deg);
  }
  20% {
    clip-path: polygon(0 15%, 100% 15%, 100% 15%, 0 15%);
    transform: translate(-5px) skew(-2deg);
  }
  30% {
    clip-path: polygon(0 10%, 100% 10%, 100% 20%, 0 20%);
    transform: translate(5px) skew(2deg);
  }
  40% {
    clip-path: polygon(0 1%, 100% 1%, 100% 2%, 0 2%);
    transform: translate(-5px) skew(-1deg);
  }
  50% {
    clip-path: polygon(0 33%, 100% 33%, 100% 33%, 0 33%);
    transform: translate(0) skew(0deg);
  }
  55% {
    clip-path: polygon(0 44%, 100% 44%, 100% 44%, 0 44%);
    transform: translate(5px) skew(1deg);
  }
  60% {
    clip-path: polygon(0 50%, 100% 50%, 100% 20%, 0 20%);
    transform: translate(-5px) skew(-2deg);
  }
  65% {
    clip-path: polygon(0 70%, 100% 70%, 100% 70%, 0 70%);
    transform: translate(5px) skew(1deg);
  }
  70% {
    clip-path: polygon(0 80%, 100% 80%, 100% 80%, 0 80%);
    transform: translate(-5px) skew(-3deg);
  }
  75% {
    clip-path: polygon(0 50%, 100% 50%, 100% 55%, 0 55%);
    transform: translate(0) skew(0deg);
  }
  80% {
    clip-path: polygon(0 70%, 100% 70%, 100% 80%, 0 80%);
    transform: translate(-5px) skew(-2deg);
  }
  85% {
    clip-path: polygon(0 10%, 100% 10%, 100% 10%, 0 10%);
    transform: translate(5px) skew(2deg);
  }
  90% {
    clip-path: polygon(0 30%, 100% 30%, 100% 30%, 0 30%);
    transform: translate(0) skew(0deg);
  }
  95% {
    clip-path: polygon(0 88%, 100% 88%, 100% 88%, 0 88%);
    transform: translate(-5px) skew(-1deg);
  }
  100% {
    clip-path: polygon(0 70%, 100% 70%, 100% 70%, 0 70%);
    transform: translate(0) skew(0deg);
  }
}

.VPFeatures {
  position: relative;
  background: radial-gradient(circle at 50% 50%, rgba(0, 255, 0, 0.1), transparent);
}

.VPFeatures .box {
  border: 1px solid rgba(0, 229, 255, 0.2);
  background: rgba(0, 0, 0, 0.2);
  backdrop-filter: blur(10px);
  transition: all 0.3s ease;
}

.VPFeatures .box:hover {
  border-color: #00ff00;
  box-shadow: 0 0 20px rgba(0, 255, 0, 0.3);
  transform: translateY(-5px);
}


.VPFeatures .details {
  color: rgba(255, 255, 255, 0.8);
}

.VPButton.brand {
  background: linear-gradient(90deg, #00ff00, #00e5ff);
  border: none;
  position: relative;
  overflow: hidden;
}

.VPButton.brand::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: linear-gradient(
    45deg,
    transparent,
    rgba(255, 255, 255, 0.1),
    transparent
  );
  transform: rotate(45deg);
  animation: shine 3s infinite;
}

@keyframes shine {
  0% {
    transform: translateX(-100%) rotate(45deg);
  }
  100% {
    transform: translateX(100%) rotate(45deg);
  }
}
</style>