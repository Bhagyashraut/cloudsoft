# cloudsoft
{
  "server": {
    "host": "example.com",
    "port": 443,
    "protocol": "https",
    "ssl": {
      "enabled": true,
      "certificate": "/path/to/certificate.pem",
      "private_key": "/path/to/private-key.pem",
      "ca_certificate": "/path/to/ca-certificate.pem"
    }
  },
  "security": {
    "hsts": {
      "enabled": true,
      "max_age": 31536000,
      "include_subdomains": true,
      "preload": true
    },
    "content_security_policy": "default-src 'self'; script-src 'self' 'unsafe-inline'",
    "x_frame_options": "DENY",
    "x_content_type_options": "nosniff",
    "referrer_policy": "strict-origin-when-cross-origin"
  },
  "redirects": {
    "http_to_https": true
  }
}

