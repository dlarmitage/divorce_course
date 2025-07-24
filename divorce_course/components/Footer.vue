<template>
  <div class="footer">
    <!-- Top border lines -->
    <div class="border-line top-left"></div>
    <div class="border-line top-right"></div>
    <div class="border-line left"></div>
    <div class="border-line right"></div>
    
    <!-- Footer content -->
    <div class="footer-content">
      <!-- Logo and organization name -->
      <div class="footer-left">
        <a href="https://careforthekid.com" target="_blank" class="logo-link" style="text-decoration: none !important;">
          <img src="/logo.png" alt="Care for the Kids Logo" class="logo-image" />
        </a>
      </div>
      
      <!-- Copyright -->
      <div class="footer-center">
        <span class="copyright">© 2025 The Connected Family LLC. All rights reserved.</span>
      </div>
      
      <!-- Organization name -->
      <div class="footer-right">
        <a href="https://careforthekid.com" target="_blank" class="org-link" style="text-decoration: none !important;">
          Care for the Kids
        </a>
      </div>
    </div>
  </div>
</template>

<script setup>
// No additional logic needed for this component
</script>

<style scoped>
/* Force remove all underlines from footer links */
.footer a,
.footer a:hover,
.footer a:focus,
.footer a:visited,
.footer a:active {
  text-decoration: none !important;
  text-decoration-line: none !important;
  text-decoration-style: none !important;
  text-decoration-color: transparent !important;
  text-decoration-thickness: 0 !important;
  border-bottom: none !important;
  box-shadow: none !important;
}
.footer {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  height: 60px;
  background: white;
  z-index: 100;
}

/* Border lines */
.border-line {
  position: absolute;
  background: #4EC5D4;
  opacity: 0.3;
}

.top-left {
  top: 0;
  left: 0;
  width: 30%;
  height: 1px;
}

.top-right {
  top: 0;
  right: 0;
  width: 30%;
  height: 1px;
}

.left {
  top: 0;
  left: 0;
  width: 1px;
  height: 30%;
}

.right {
  top: 0;
  right: 0;
  width: 1px;
  height: 30%;
}

/* Footer content */
.footer-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100%;
  padding: 0 20px;
  max-width: 1200px;
  margin: 0 auto;
}

/* Logo */
.logo-link {
  text-decoration: none !important;
  text-decoration-line: none !important;
  text-decoration-style: none !important;
  text-decoration-color: transparent !important;
  display: flex;
  align-items: center;
}

.logo-image {
  width: 40px;
  height: 40px;
  object-fit: contain;
  transition: transform 0.3s ease;
}

.logo-link:hover .logo-image {
  transform: scale(1.05);
}

.logo-link:hover {
  text-decoration: none !important;
  text-decoration-line: none !important;
}

/* Copyright */
.copyright {
  color: #888;
  font-size: 8px;
  font-weight: 300;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Arial, sans-serif;
}

/* Organization name */
.org-link {
  color: #36747b;
  text-decoration: none !important;
  text-decoration-line: none !important;
  text-decoration-style: none !important;
  text-decoration-color: transparent !important;
  font-size: 14px;
  font-weight: 500;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  transition: color 0.3s ease;
}

.org-link:hover {
  color: #146b8c;
  text-decoration: none !important;
  text-decoration-line: none !important;
}

/* Global footer link styling */
.footer a {
  text-decoration: none !important;
  text-decoration-line: none !important;
  text-decoration-style: none !important;
  text-decoration-color: transparent !important;
}

.footer a:hover {
  text-decoration: none !important;
  text-decoration-line: none !important;
}

/* Responsive adjustments */
@media (max-width: 768px) {
  .footer-content {
    padding: 0 15px;
  }
  
  .copyright {
    font-size: 10px;
  }
  
  .org-link {
    font-size: 12px;
  }
}
</style> 