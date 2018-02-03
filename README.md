SEND A TEST MESSAGE
===================

````
require 'base64'
require 'socket'

payload = "gwVGQRhJiAEBAQIAcVTp/X1U6f1+E5sWtsY1YYQAACl3AAAABQASCSIQF/+h\nDwsIAARlEAAAFc0vAAAxowAASXoAZR6/AAEZdQABYvsAZXfXAAAAEQBm2sEA\nAAaXAAAAAAAAAAAAAAAAAAAAAAAAAGkAAAAB\n"

UDPSocket.new.send(Base64.decode64(payload), 0, '127.0.0.1', '11100')
````