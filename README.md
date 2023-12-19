# RJPOLICE_HACK_836_TechExplorers_5
# PHISHGUARD
## OVERVIEW
The HTML script you provided is a simple client-side phishing detection mechanism. It checks whether the current website's URL matches any of the trusted URLs in the trustedURLs array. If a match is found, it alerts the user that the website is trusted; otherwise, it alerts that the website may not be trusted.
## Usage
<!DOCTYPE html>
<html>
<head>
  <title>Phishing Detection</title>
  <script>
    function checkURL() {
      var trustedURLs = [
        "https://www.trustedwebsite1.com",
        "https://www.trustedwebsite2.com"
        // Add more trusted URLs to this list
      ];

      var currentURL = window.location.href;

      for (var i = 0; i < trustedURLs.length; i++) {
        if (currentURL === trustedURLs[i]) {
          alert("This website is trusted.");
          return;
        }
      }

      alert("This website may not be trusted.");
    }
  </script>
</head>
<body onload="checkURL()">
  <!-- Your website content goes here -->
</body>
</html>

## Contributing
Contributions are welcome! If you find issues or have suggestions for improvements, please open an issue or submit a pull request.
