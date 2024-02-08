The objective of a project focused on developing a currency conversion service  is to create a client-server application that allows users to easily convert one currency (provided by the users) to another over a network, such as the internet.
 ** IMPLEMENTATION**
1.Client-Server Architecture:
A client-server architecture has been established using Python's socket module for communication. This allows the client and server to exchange data over a TCP connection.

2.Client GUI (client.py):
A graphical user interface (GUI) has been created for the client using the tkinter library.
Users can input data in the GUI interface.




SERVER IMPLEMENTATION:

1.Set Up a Server Socket: 
    Create a TCP server socket to listen for incoming client connections. 
2.Exchange Rate Data: 
    Obtain up-to-date exchange rate data from a reliable source.
3.Process Client Requests: 
    Continuously listen for incoming client connections and accept them. When a connection is accepted, the server reads the client's request, which should include the amount, source currency, and target currency.

4.Currency Conversion: 
    Use the exchange rate data to perform the currency conversion. 
5.Send the Result to the Client: 
    Send the converted amount back to the client over the established TCP connection.




CLIENT IMPLEMENTATION:

1.Set Up a Client Socket: 
    Create a TCP client socket and connect it to the server's IP address and port.

2.Send a Request: 
    When the user initiates a request, format the request data and send it to the server over the TCP connection.

3.Receive and Display the Result: 
    Once the request is sent, the client waits for the server's response. Upon receiving the response, display the converted amount to the user.



