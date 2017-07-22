Protobuf Logging Reference
==========================

.. class:: DNSDistProtoBufMessage

  This object represents a single protobuf message as emitted by :program:`dnsdist`.

.. classmethod:: DNSDistProtoBufMessage:setBytes(bytes)

  Set the size of the query

  :param int bytes: Number of bytes in the query.

.. classmethod:: DNSDistProtoBufMessage:setEDNSSubnet(netmask)

  Set the EDNS Subnet to ``netmask``.

  :param string netmask: The netmask to set to.

.. classmethod:: DNSDistProtoBufMessage:setQueryTime(sec, usec)

  In a response message, set the time at which the query has been received.

  :param int sec: Unix timestamp when the query was received.
  :param int usec: The microsecond the query was received.

.. classmethod:: DNSDistProtoBufMessage:setQuestion(name, qtype, qclass)

  Set the question in the protobuf message.

  :param DNSName name: The qname of the question
  :param int qtype: The qtype of the question
  :param int qclass: The qclass of the question

.. classmethod:: DNSDistProtoBufMessage:setRequestor(address)

  Set the requestor's address.

  :param ComboAddress address: The address to set to

.. classmethod:: DNSDistProtoBufMessage:setRequestorFromString(address)

  Set the requestor's address from a string.

  :param string address: The address to set to

.. classmethod:: DNSDistProtoBufMessage:setResponder(address)

  Set the responder's address.

  :param ComboAddress address: The address to set to

.. classmethod:: DNSDistProtoBufMessage:setResponderFromString(string)

  Set the responder's address.

  :param string address: The address to set to

.. classmethod:: DNSDistProtoBufMessage:setResponseCode(rcode)

  Set the response code of the query.

  :param int rcode: The response code of the answer

.. classmethod:: DNSDistProtoBufMessage:setTime(sec, usec)

  Set the time at which the query or response has been received.

  :param int sec: Unix timestamp when the query was received.
  :param int usec: The microsecond the query was received.

.. classmethod:: DNSDistProtoBufMessage:toDebugString() -> string

  Return an string containing the content of the message
