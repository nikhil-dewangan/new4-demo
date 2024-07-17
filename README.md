# Definition: 
The Internet is a global network of interconnected networks that use standardized 
communication protocols (TCP/IP) to link billions of devices worldwide. It is a network of networks.

# new4-demo
In summary, synchronous communication and processes require real-time, simultaneous interaction, while asynchronous communication and processes allow for, 
independent timing and flexibility, with interactions occurring at different times.
1. Header
   The header typically consists of two parts:

* Type of token: JWT,
* Algorithm used: For example, HMAC SHA256 or RSA

2. Payload
   The payload contains the claims. Claims are statements about an entity (typically, the user) and additional data. There are three types of claims:

* Registered claims: These are predefined claims which are not mandatory but recommended, like iss (issuer), exp (expiration time), sub (subject), aud (audience), etc.
* Public claims: These can be defined at will by those using JWTs but should be collision-resistant.
* Private claims: Custom claims created to share information between parties that agree on using them.

3. Signature
   To create the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

# Security Considerations.

1. Secret Key: The secret key used to sign the JWT must be kept safe. If someone gets hold of it, they can create valid tokens.

2. Expiration: Always set an expiration for the JWT to reduce the risk of it being used indefinitely.

3. Transport Security: Always use HTTPS to prevent tokens from being intercepted in transit.

4. Algorithm Choice: Be cautious of the algorithm used to sign the JWT. Some algorithms are more secure than others.

var ReactDebugCurrentFrame = {};
  var currentExtraStackFrame = null;
  function setExtraStackFrame(stack) {
    {
      currentExtraStackFrame = stack;
    }
  }
  {
    ReactDebugCurrentFrame.setExtraStackFrame = function (stack) {
      {
        currentExtraStackFrame = stack;
      }
    }; // Stack implementation injected by the current renderer.

   
    ReactDebugCurrentFrame.getCurrentStack = null;

    ReactDebugCurrentFrame.getStackAddendum = function () {
      var stack = ''; // Add an extra top frame while an element is being validated

      if (currentExtraStackFrame) {
        stack += currentExtraStackFrame;
      } // Delegate to the injected renderer-specific implementation


      var impl = ReactDebugCurrentFrame.getCurrentStack;

      if (impl) {
        stack += impl() || '';
      }

      return stack;
    };

    // -----------------------------------------------------------------------------

  var enableScopeAPI = false; // Experimental Create Event Handle API.
  var enableCacheElement = false;
  var enableTransitionTracing = false; // No known bugs, but needs performance testing

  var enableLegacyHidden = false; // Enables unstable_avoidThisFallback feature in Fiber
  // stuff. Intended to enable React core members to more easily debug scheduling
  // issues in DEV builds.

  An object literal is a list of name:value pairs inside curly braces {}.
  {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"}.





