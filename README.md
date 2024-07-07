# new4-demo
In summary, synchronous communication and processes require real-time, simultaneous interaction, while asynchronous communication and processes allow for, 
independent timing and flexibility, with interactions occurring at different times.
1. Header
   The header typically consists of two parts:

* Type of token: JWT
* Algorithm used: For example, HMAC SHA256 or RSA

2. Payload
   The payload contains the claims. Claims are statements about an entity (typically, the user) and additional data. There are three types of claims:

* Registered claims: These are predefined claims which are not mandatory but recommended, like iss (issuer), exp (expiration time), sub (subject), aud (audience), etc.
* Public claims: These can be defined at will by those using JWTs but should be collision-resistant.
* Private claims: Custom claims created to share information between parties that agree on using them.

3. Signature
To create the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

#Security Considerations.

1. Secret Key: The secret key used to sign the JWT must be kept safe. If someone gets hold of it, they can create valid tokens.

2. Expiration: Always set an expiration for the JWT to reduce the risk of it being used indefinitely.

3. Transport Security: Always use HTTPS to prevent tokens from being intercepted in transit.

4. Algorithm Choice: Be cautious of the algorithm used to sign the JWT. Some algorithms are more secure than others.


});





