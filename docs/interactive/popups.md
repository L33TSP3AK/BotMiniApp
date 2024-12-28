# Popup Variations

Explore different styles and types of popup components.

## Basic Popup

<div class="popup-demo">
  <button class="popup-trigger" onclick="document.getElementById('basic-popup').classList.add('active')">
    Basic Popup
  </button>
  
  <div id="basic-popup" class="popup">
    <div class="popup-content basic">
      <button class="close-btn" onclick="document.getElementById('basic-popup').classList.remove('active')">×</button>
      <h3>Basic Popup</h3>
      <p>A simple popup with basic styling.</p>
    </div>
  </div>
</div>

## Slide Popup

<div class="popup-demo">
  <button class="popup-trigger" onclick="document.getElementById('slide-popup').classList.add('active')">
    Slide Popup
  </button>
  
  <div id="slide-popup" class="popup slide">
    <div class="popup-content">
      <button class="close-btn" onclick="document.getElementById('slide-popup').classList.remove('active')">×</button>
      <h3>Slide Popup</h3>
      <p>This popup slides in from the top.</p>
    </div>
  </div>
</div>

## Scale Popup

<div class="popup-demo">
  <button class="popup-trigger" onclick="document.getElementById('scale-popup').classList.add('active')">
    Scale Popup
  </button>
  
  <div id="scale-popup" class="popup scale">
    <div class="popup-content">
      <button class="close-btn" onclick="document.getElementById('scale-popup').classList.remove('active')">×</button>
      <h3>Scale Popup</h3>
      <p>This popup scales up when appearing.</p>
    </div>
  </div>
</div>

## Rotate Popup

<div class="popup-demo">
  <button class="popup-trigger" onclick="document.getElementById('rotate-popup').classList.add('active')">
    Rotate Popup
  </button>
  
  <div id="rotate-popup" class="popup rotate">
    <div class="popup-content">
      <button class="close-btn" onclick="document.getElementById('rotate-popup').classList.remove('active')">×</button>
      <h3>Rotate Popup</h3>
      <p>This popup rotates into view.</p>
    </div>
  </div>
</div>

## Flip Popup

<div class="popup-demo">
  <button class="popup-trigger" onclick="document.getElementById('flip-popup').classList.add('active')">
    Flip Popup
  </button>
  
  <div id="flip-popup" class="popup flip">
    <div class="popup-content">
      <button class="close-btn" onclick="document.getElementById('flip-popup').classList.remove('active')">×</button>
      <h3>Flip Popup</h3>
      <p>This popup flips into position.</p>
    </div>
  </div>
</div>

## Swing Popup

<div class="popup-demo">
  <button class="popup-trigger" onclick="document.getElementById('swing-popup').classList.add('active')">
    Swing Popup
  </button>
  
  <div id="swing-popup" class="popup swing">
    <div class="popup-content">
      <button class="close-btn" onclick="document.getElementById('swing-popup').classList.remove('active')">×</button>
      <h3>Swing Popup</h3>
      <p>This popup swings into view.</p>
    </div>
  </div>
</div>

## Slide Side Popup

<div class="popup-demo">
  <button class="popup-trigger" onclick="document.getElementById('slide-side-popup').classList.add('active')">
    Slide Side
  </button>
  
  <div id="slide-side-popup" class="popup slide-side">
    <div class="popup-content">
      <button class="close-btn" onclick="document.getElementById('slide-side-popup').classList.remove('active')">×</button>
      <h3>Slide Side Popup</h3>
      <p>This popup slides in from the side.</p>
    </div>
  </div>
</div>

## Bounce Popup

<div class="popup-demo">
  <button class="popup-trigger" onclick="document.getElementById('bounce-popup').classList.add('active')">
    Bounce Popup
  </button>
  
  <div id="bounce-popup" class="popup bounce">
    <div class="popup-content">
      <button class="close-btn" onclick="document.getElementById('bounce-popup').classList.remove('active')">×</button>
      <h3>Bounce Popup</h3>
      <p>This popup bounces into view.</p>
    </div>
  </div>
</div>

## Fade Rotate Popup

<div class="popup-demo">
  <button class="popup-trigger" onclick="document.getElementById('fade-rotate-popup').classList.add('active')">
    Fade Rotate
  </button>
  
  <div id="fade-rotate-popup" class="popup fade-rotate">
    <div class="popup-content">
      <button class="close-btn" onclick="document.getElementById('fade-rotate-popup').classList.remove('active')">×</button>
      <h3>Fade Rotate Popup</h3>
      <p>This popup fades and rotates into view.</p>
    </div>
  </div>
</div>

## Zoom Blur Popup

<div class="popup-demo">
  <button class="popup-trigger" onclick="document.getElementById('zoom-blur-popup').classList.add('active')">
    Zoom Blur
  </button>
  
  <div id="zoom-blur-popup" class="popup zoom-blur">
    <div class="popup-content">
      <button class="close-btn" onclick="document.getElementById('zoom-blur-popup').classList.remove('active')">×</button>
      <h3>Zoom Blur Popup</h3>
      <p>This popup zooms in with a blur effect.</p>
    </div>
  </div>
</div>

<style>
.popup-demo {
  display: inline-block;
  margin: 0.5rem;
}

.popup-trigger {
  padding: 0.5rem 1rem;
  background: var(--vp-c-brand);
  color: white;
  border: none;
  border-radius: 0.25rem;
  cursor: pointer;
  transition: all 0.3s ease;
}

.popup-trigger:hover {
  background: var(--vp-c-brand-dark);
  transform: translateY(-2px);
}

.popup {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.8);
  backdrop-filter: blur(4px);
  display: flex;
  align-items: center;
  justify-content: center;
  opacity: 0;
  pointer-events: none;
  transition: all 0.3s ease;
}

.popup.active {
  opacity: 1;
  pointer-events: auto;
}

.popup-content {
  background: var(--vp-c-bg-soft);
  padding: 2rem;
  border-radius: 0.75rem;
  max-width: 500px;
  width: 90%;
  position: relative;
  border: 1px solid var(--vp-c-brand);
}

.close-btn {
  position: absolute;
  top: 1rem;
  right: 1rem;
  background: none;
  border: none;
  color: var(--vp-c-text-2);
  font-size: 1.5rem;
  cursor: pointer;
  padding: 0;
  line-height: 1;
}

.close-btn:hover {
  color: var(--vp-c-text-1);
}

/* Slide Animation */
.popup.slide .popup-content {
  transform: translateY(-100%);
  transition: transform 0.3s ease;
}

.popup.slide.active .popup-content {
  transform: translateY(0);
}

/* Scale Animation */
.popup.scale .popup-content {
  transform: scale(0.7);
  transition: transform 0.3s ease;
}

.popup.scale.active .popup-content {
  transform: scale(1);
}

/* Rotate Animation */
.popup.rotate .popup-content {
  transform: rotate(-180deg) scale(0);
  transition: all 0.3s ease;
}

.popup.rotate.active .popup-content {
  transform: rotate(0) scale(1);
}

/* Flip Animation */
.popup.flip .popup-content {
  transform: perspective(1000px) rotateX(-90deg);
  transition: all 0.3s ease;
  transform-origin: top center;
}

.popup.flip.active .popup-content {
  transform: perspective(1000px) rotateX(0);
}

/* Swing Animation */
.popup.swing .popup-content {
  transform: perspective(1000px) rotateY(-90deg);
  transition: all 0.3s ease;
  transform-origin: center right;
}

.popup.swing.active .popup-content {
  transform: perspective(1000px) rotateY(0);
}

/* Slide Side Animation */
.popup.slide-side .popup-content {
  transform: translateX(-100%);
  transition: transform 0.3s ease;
}

.popup.slide-side.active .popup-content {
  transform: translateX(0);
}

/* Bounce Animation */
@keyframes bounceIn {
  0% { transform: scale(0.3); opacity: 0; }
  50% { transform: scale(1.05); opacity: 0.8; }
  70% { transform: scale(0.9); opacity: 0.9; }
  100% { transform: scale(1); opacity: 1; }
}

.popup.bounce .popup-content {
  opacity: 0;
}

.popup.bounce.active .popup-content {
  animation: bounceIn 0.6s cubic-bezier(0.68, -0.55, 0.265, 1.55);
  opacity: 1;
}

/* Fade Rotate Animation */
.popup.fade-rotate .popup-content {
  transform: rotate(-720deg) scale(0);
  opacity: 0;
  transition: all 0.5s ease;
}

.popup.fade-rotate.active .popup-content {
  transform: rotate(0) scale(1);
  opacity: 1;
}

/* Zoom Blur Animation */
.popup.zoom-blur .popup-content {
  transform: scale(2);
  filter: blur(10px);
  opacity: 0;
  transition: all 0.3s ease;
}

.popup.zoom-blur.active .popup-content {
  transform: scale(1);
  filter: blur(0);
  opacity: 1;
}
</style>
```
</boltArtifact>

I've created 10 different popup variations with unique animations and effects:

1. Basic Popup - Simple fade in/out
2. Slide Popup - Slides in from top
3. Scale Popup - Scales up from center
4. Rotate Popup - Rotates into view
5. Flip Popup - Flips in from top
6. Swing Popup - Swings in from side
7. Slide Side Popup - Slides in from left
8. Bounce Popup - Bounces into view
9. Fade Rotate Popup - Fades in while rotating
10. Zoom Blur Popup - Zooms in with blur effect

Each popup features:
- Smooth animations
- Backdrop blur
- Close button
- Responsive design
- Dark theme compatibility
- Border accents
- Hover effects on triggers

The popups use CSS transforms and transitions for smooth performance and can be easily custom