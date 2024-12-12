# Authentication

<script src="https://identity.netlify.com/v1/netlify-identity-widget.js"></script>

<div id="login-container">
  <button id="login-btn" onclick="netlifyIdentity.open()">Login</button>
</div>

<script>
  // Initialize Netlify Identity
  netlifyIdentity.init();

  // Handle login event
  netlifyIdentity.on('login', user => {
    netlifyIdentity.close();
    // Redirect to home page after successful login
    window.location.href = '/';
  });

  // Check current user on page load
  document.addEventListener('DOMContentLoaded', function() {
    const user = netlifyIdentity.currentUser();
    
    if (user) {
      // Hide login button if user is already logged in
      document.getElementById('login-container').style.display = 'none';
    }
  });

  // Optional: Add logout functionality
  function logout() {
    netlifyIdentity.logout();
  }

  // Handle logout event
  netlifyIdentity.on('logout', () => {
    // Redirect to login page after logout
    window.location.href = '/login.md';
  });
</script>