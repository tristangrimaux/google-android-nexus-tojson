# google-android-nexus-tojson

This quick shell command line script returns in a JSON format the nexus images available in the page https://developers.google.com/android/nexus/images

I use it to get latest version for the Nexus 6, codename shamu in this way

google-android-nexus-images | jq -r '.[-1]|select(.id == "shamu")|.data.version'

To install just copy the file, make it executable and make sure you have the tools xml2json and jq installed in your system


