====================
Twisted Network Programming Essentials, 2E
====================

Part I. An Introduction to Twisted
====================

CHAPTER 1. Getting Started
--------------------

 1. Installing Twisted

     a. For convenience I install a package ipython:
        
        **pip install ipython**

     b. Install twisted:
     
        **pip install twisted**


 2. Installing from Source

 3. Testing Your Installation

     $ ipython

     >>> import twisted

     >>> twisted.__version__


 4. Using the Twisted Documentation

     `Documentation`_

     .. _Documentation: http://twistedmatrix.com/trac/wiki/Documentation

 5. Finding Answers to Your Questions

     `stackoverflow`_

     .. _stackoverflow: http://stackoverflow.com/questions/tagged/twisted

     `Twisted Blogs`_

     .. _Twisted Blods: http://labs.twistedmatrix.com/


CHAPTER 2 Building Basic Clients and Servers
--------------------

 1. A TCP Echo Server and Client
      
     Exmple 2-1. echoserver.py::

       from twisted.internet import protocol, reactor

       class Echo(protocol.Protocol):
           def dataReceived(self, data):
               self.transport.write(data)


       class EchoFactory(protocol.Factory):
           def buildProtocol(self, addr):
               return Echo()


       reactor.listenTCP(8000, EchoFactory())
       reactor.run()

     Example 2-2. echoclient.py::
       
       from twisted.internet import reactor, protocol


       class EchoClient(protocol.Protocol):
           def connectionMade(self):
               self.transport.write("Hello, world!")


           def dataReceived(self, data):
               print "Server said:", data
                   self.transport.loseConnection()


       class EchoFactory(protocol.ClientFactory):
           def buildProtocol(self, addr):
               return EchoClient()

           def clientConnectionFailed(self, connector, reason):
               print "Connection failed."
               reactor.stop()
               
           def clientConnectionLost(self, connector, reason):
               print "Connection lost."
               reactor.stop()
               
       reactor.connectTCP("localhost", 8000, EchoFactory())
       reactor.run()


 2. Event-Driven Programming

 3. The Reactor

 4. Transports

 5. Protocols

 6. A TCP Quote Server and Client

 7. Protocol State Machines

 8. More Practice and Next Steps


PART II. Building Production-GradeBuilding Twisted Services
====================


PART III. More Protocols and More Practice
====================
