# Alert Styles

Different styles of alerts to highlight important information.

## Basic Alerts

<div class="alert alert-info">
  <div class="alert-icon">ℹ️</div>
  <div class="alert-content">
    <h4>Information</h4>
    <p>This is a basic information alert.</p>
  </div>
</div>

<div class="alert alert-success">
  <div class="alert-icon">✅</div>
  <div class="alert-content">
    <h4>Success</h4>
    <p>Operation completed successfully.</p>
  </div>
</div>

<div class="alert alert-warning">
  <div class="alert-icon">⚠️</div>
  <div class="alert-content">
    <h4>Warning</h4>
    <p>Please proceed with caution.</p>
  </div>
</div>

<div class="alert alert-danger">
  <div class="alert-icon">🚫</div>
  <div class="alert-content">
    <h4>Error</h4>
    <p>Something went wrong.</p>
  </div>
</div>

<style>
.alert {
  display: flex;
  gap: 1rem;
  padding: 1rem;
  border-radius: 0.5rem;
  margin: 1rem 0;
}

.alert-icon {
  font-size: 1.5rem;
}

.alert-content h4 {
  margin: 0 0 0.5rem 0;
}

.alert-content p {
  margin: 0;
}

.alert-info {
  background: #e0f2fe;
  border-left: 4px solid #0ea5e9;
}

.alert-success {
  background: #dcfce7;
  border-left: 4px solid #22c55e;
}

.alert-warning {
  background: #fef3c7;
  border-left: 4px solid #f59e0b;
}

.alert-danger {
  background: #fee2e2;
  border-left: 4px solid #ef4444;
}
</style>