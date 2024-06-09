<h2>Portscanner</h2>
<p>This project implements a basic port scanner using Python's socket module. It scans a specified remote host to identify open ports.</p>
<h3>Key Functionalities:</h3>
    <p><b>User Input</b>: Prompts the user to enter the hostname or IP address of the target machine.</p>
    <p><b>IP Resolution</b>: Converts the hostname to its corresponding IP address using socket.gethostbyname.</p>
    <p><b>Port Scanning Loop:</b>Iterates through a range of ports (typically 1-1024).</p>
    <p><b>Socket Creation:</b> Creates a TCP socket object for each port using socket.socket.</p>
    <p><b>Connection Attempt:</b>Attempts to connect to the specified port on the remote host using socket.connect_ex.</p>
    <p><b>Open Port Detection:</b> Checks the connection attempt result. If successful (result is 0), the port is considered open and its number is printed.</p>
    <p><b>Error Handling:</b>Handles exceptions like KeyboardInterrupt (user presses Ctrl+C), socket.gaierror (hostname resolution failure), and socket.error (generic socket error).</p>
    <p><b>Scan Duration</b>:Calculates the total time taken to scan the ports using timestamps.</p>
