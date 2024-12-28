# Notifications

Toast and notification components for user feedback.

## Toast Notifications

<div class="notification-container">
  <button class="show-notification" onclick="document.getElementById('toast-demo').classList.add('show')">
    Show Toast
  </button>
  
  <div id="toast-demo" class="toast" onclick="this.classList.remove('show')">
    <div class="toast-icon">✅</div>
    <div class="toast-content">
      <h4>Success</h4>
      <p>Operation completed successfully</p>
    </div>
  </div>
</div>

## Notification Types

<div class="notification success">
  <div class="notification-icon">✅</div>
  <div class="notification-content">
    <h4>Success Message</h4>
    <p>Your changes have been saved.</p>
  </div>
  <button class="notification-close">×</button>
</div>

<div class="notification info">
  <div class="notification-icon">ℹ️</div>
  <div class="notification-content">
    <h4>Information</h4>
    <p>Updates are available for your system.</p>
  </div>
  <button class="notification-close">×</button>
</div>

<div class="notification warning">
  <div class="notification-icon">⚠️</div>
  <div class="notification-content">
    <h4>Warning</h4>
    <p>Please backup your data before continuing.</p>
  </div>
  <button class="notification-close">×</button>
</div>

<style>
.notification-container {
  margin: 2rem 0;
}

.show-notification {
  padding: 0.5rem 1rem;
  background: var(--vp-c-brand);
  color: white;
  border: none;
  border-radius: 0.25rem;
  cursor: pointer;
}

.toast {
  position: fixed;
  bottom: 1rem;
  right: 1rem;
  display: flex;
  gap: 1rem;
  padding: 1rem;
  background: white;
  border-radius: 0.5rem;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
  opacity: 0;
  transform: translateY(1rem);
  transition: all 0.3s ease;
  cursor: pointer;
}

.toast.show {
  opacity: 1;
  transform: translateY(0);
}

.notification {
  display: flex;
  gap: 1rem;
  align-items: start;
  padding: 1rem;
  border-radius: 0.5rem;
  margin: 1rem 0;
  animation: slideIn 0.3s ease;
}

.notification-icon {
  font-size: 1.25rem;
}

.notification-content {
  flex: 1;
}

.notification-content h4 {
  margin: 0 0 0.25rem 0;
}

.notification-content p {
  margin: 0;
}

.notification-close {
  background: none;
  border: none;
  font-size: 1.5rem;
  cursor: pointer;
  padding: 0;
  opacity: 0.5;
}

.notification-close:hover {
  opacity: 1;
}

.notification.success {
  background: #f0fdf4;
  border: 1px solid #22c55e;
}

.notification.info {
  background: #e0f2fe;
  border: 1px solid #0ea5e9;
}

.notification.warning {
  background: #fef3c7;
  border: 1px solid #f59e0b;
}

@keyframes slideIn {
  from {
    opacity: 0;
    transform: translateX(1rem);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}
</style>