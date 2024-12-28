# Toast Notifications

<BackToAdmin />

<div class="toast-demo">
  <div class="demo-grid">
    <div class="demo-card">
      <h3>Slide Animation</h3>
      <p>Smooth slide-in from the right</p>
      <button class="demo-button" onclick="window.$vueApp.showToast({
        message: 'Sliding in from the right',
        type: 'info',
        animation: 'slide'
      })">Show Toast</button>
    </div>
    <div class="demo-card">
      <h3>Fade Animation</h3>
      <p>Simple fade in/out effect</p>
      <button class="demo-button" onclick="window.$vueApp.showToast({
        message: 'Fading in and out smoothly',
        type: 'success',
        animation: 'fade'
      })">Show Toast</button>
    </div>
    <div class="demo-card">
      <h3>Bounce Animation</h3>
      <p>Bouncy scale animation</p>
      <button class="demo-button" onclick="window.$vueApp.showToast({
        message: 'Bouncing into view!',
        type: 'warning',
        animation: 'bounce'
      })">Show Toast</button>
    </div>
    <div class="demo-card">
      <h3>Flip Animation</h3>
      <p>3D flip effect</p>
      <button class="demo-button" onclick="window.$vueApp.showToast({
        message: 'Flipping in 3D space',
        type: 'error',
        animation: 'flip'
      })">Show Toast</button>
    </div>
    <div class="demo-card">
      <h3>Zoom Animation</h3>
      <p>Scale in/out effect</p>
      <button class="demo-button" onclick="window.$vueApp.showToast({
        message: 'Zooming into position',
        type: 'info',
        animation: 'zoom'
      })">Show Toast</button>
    </div>
    <div class="demo-card">
      <h3>Rotate Animation</h3>
      <p>Rotating scale effect</p>
      <button class="demo-button" onclick="window.$vueApp.showToast({
        message: 'Rotating into place',
        type: 'success',
        animation: 'rotate'
      })">Show Toast</button>
    </div>
    <div class="demo-card">
      <h3>Glitch Animation</h3>
      <p>Digital glitch effect</p>
      <button class="demo-button" onclick="window.$vueApp.showToast({
        message: 'Glitching into reality',
        type: 'warning',
        animation: 'glitch'
      })">Show Toast</button>
    </div>
  </div>
</div>

<style>
.toast-demo {
  padding: 2rem;
  background: var(--vp-c-bg-soft);
  border-radius: 1rem;
  margin: 2rem 0;
}

.demo-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
}

.demo-card {
  background: var(--vp-c-bg-alt);
  border: 1px solid var(--vp-c-border);
  border-radius: 0.75rem;
  padding: 1.5rem;
  transition: all 0.3s ease;
}

.demo-card:hover {
  transform: translateY(-2px);
  border-color: var(--vp-c-brand);
  box-shadow: 0 4px 12px rgba(0, 229, 255, 0.1);
}

.demo-card h3 {
  margin: 0 0 0.5rem 0;
  color: var(--vp-c-brand);
}

.demo-card p {
  margin: 0 0 1rem 0;
  color: var(--vp-c-text-2);
  font-size: 0.9rem;
}

.demo-button {
  width: 100%;
  padding: 0.75rem;
  background: var(--vp-c-brand);
  color: var(--vp-c-bg);
  border: none;
  border-radius: 0.5rem;
  cursor: pointer;
  font-weight: 600;
  transition: all 0.3s ease;
}

.demo-button:hover {
  background: var(--vp-c-brand-dark);
  transform: translateY(-2px);
}
</style>